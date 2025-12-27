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
Add Code Here
~~~
def factorial(n):
    fact = 1
    for i in range(1, n + 1):
        fact *= i
    return fact

# Function to calculate nCr
def nCr(n, r):
    return factorial(n) // (factorial(r) * factorial(n - r))

# Input number of rows
rows = int(input("Enter number of rows: "))

# Generate Pascal's Triangle
for i in range(rows):
    # Print spaces for formatting
    print(" " * (rows - i), end="")

    for j in range(i + 1):
        print(nCr(i, j), end=" ")

    print()
~~~

## Sample Output


## Result
Thus,the Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user is created successfully.

