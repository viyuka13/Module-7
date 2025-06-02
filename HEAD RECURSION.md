# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:
      def fun(n):
          if n > 0:
              fun(n-1)
              print(n)
      
      num = int(input("Enter a number: "))
      if num % 2 != 0:
          num += 1
      
      fun(num)

## OUTPUT
![image](https://github.com/user-attachments/assets/1045fcdf-c31f-4e7d-b06e-e9983a14a453)

## RESULT
This program demonstrates head recursion. The function fun(n) calls itself recursively before printing, so the output prints numbers from 1 up to n in ascending order. If the user inputs an odd number, it is incremented by 1 to make it even before calling the function.
