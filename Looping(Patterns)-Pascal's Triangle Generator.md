# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
import math

rows = int(input())

for n in range(rows):
    print(" " * (rows - n), end="")
    for k in range(n + 1):
        val = math.factorial(n) // (math.factorial(k) * math.factorial(n - k))
        print(val, end=" ")
    print()
```

## Sample Output
<img width="1284" height="577" alt="Screenshot 2026-06-01 110713" src="https://github.com/user-attachments/assets/5f4fd789-eede-47c6-896c-938f2b664b4f" />

## Result
The program prints Pascal's Triangle for the given number of rows using the factorial formula for combinations.
