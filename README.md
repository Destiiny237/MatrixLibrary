## Библиотека матриц на C++

Эта библиотека предоставляет функционал для работы с матрицами, включая: 

*   **bracket.cc:** Функции для доступа к элементам матрицы по индексам. 
*   **determinant.cc:** Функция для вычисления определителя матрицы.
*   **equal.cc:** Функция для сравнения матриц на равенство. 
*   **inverse.cc:** Функция для вычисления обратной матрицы. 
*   **mul.cc:** Функция для умножения матриц.
*   **sub.cc:** Функция для вычитания матриц. 
*   **sum.cc:** Функция для сложения матриц. 
*   **transpose.cc:** Функция для транспонирования матрицы. 

### Использование

**Включение заголовочного файла:** 
```cpp
#include "matrix.h" 
```

### Пример использования
``` cpp
#include "matrix.h"

int main() {
  // Создание матрицы 2x2 
  Matrix matrix(2, 2);

  // Установка значений элементов
  matrix(0, 0) = 1;
  matrix(0, 1) = 2;
  matrix(1, 0) = 3;
  matrix(1, 1) = 4;

  // Вычисление определителя 
  double det = matrix.determinant(); 

  // Вывод результата
  std::cout << "Определитель матрицы: " << det << std::endl;

  return 0;
}
```
