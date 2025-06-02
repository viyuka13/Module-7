# 🔁 Recursion:Palindrome Checker Using Recursion in Python

## 🎯 AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

## 💻 PROGRAM:
      def is_palindrome(word):
          if len(word) < 1:
              return True
          if word[0] == word[-1]:
              return is_palindrome(word[1:-1])
          else:
              return False
      
      input_word = input("Enter a word to check if it's a palindrome: ")
      result = is_palindrome(input_word)
      
      if result:
          print("Yes, it is a palindrome.")
      else:
          print("No, it is not a palindrome.")
## OUTPUT
![image](https://github.com/user-attachments/assets/cf9263b4-5cc1-43e0-936a-80512f12bae7)

## RESULT
The program demonstrates the use of recursion to check whether a string is a palindrome and prints the result accordingly.
