# C#-Homework

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

Вычислить значение полинома (1/a)*(1/(a+2))*(1/(a+4)))..., где a = любое число

```csharp
using System;

class HelloWorld {
  static void Main() {
      
    double a = 1; // здесь введите число отличное от нуля ( на 0 делить нельзя же :) )
    int b = 2; // здесь ввести количество множителей
    
    
    if (a == 0) {
          throw new ArgumentException("Нельзя делить на 0");
      }
    
    double rsl = ((double) 1 / a) * ((double) 1 / calculatePolinom(a, b));
    
    Console.WriteLine(Math.Round(rsl, 3));
  }
  
  static double calculatePolinom(double a, int numberOfMultipliers) {
      
      double result = 1;
      
      for (int i = 1; i <= numberOfMultipliers; i++) {
          result *= a + (i * 2);
      }
      
      return result;
  }
}
```
