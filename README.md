# C-Homework

Только отрицательные числа из диапазона от A до B в обратном порядке.

```csharp
using System;

class HelloWorld {
  static void Main() {
    int a = -22; // здесь ввести последнее число из диапазона
    int b = -6; // здесь ввести начальное число из диапазона
    for (int i = a; i <= b; i++) {
        if (i % 2 == 0) {
            Console.WriteLine(i);
        }
    }
  }
}
``` 

