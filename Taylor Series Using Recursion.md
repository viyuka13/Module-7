# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## 💻 PROGRAM:
      def series(x, n):
          if n == 0:
              return 1
          else:
              return x**n / n + series(x, n - 1)
      
      x = float(input("Enter the value of x: "))
      n = int(input("Enter the value of n: "))
      result = series(x, n)
      print("Result of the series:", result)

## OUTPUT
![image](https://github.com/user-attachments/assets/68657727-ca0c-441f-9908-3b9ff321f9d0)

## RESULT
The program demonstrates the use of recursion to compute the value of the series xⁿ/n + xⁿ⁻¹/(n-1) + ... + x¹/1 + 1 and prints the result accordingly.
