# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

## 🎯 Aim:

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.



## 🧠 Algorithm:
```
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
```
## 🧪 Program:
```
def generate_pascals_triangle(n):
    triangle = []  # Initialize empty list to store rows
    for i in range(n):
        row = [1]  # First element of each row is 1
        if triangle:  # From the second row onwards
            last_row = triangle[-1]
            row.extend([last_row[j] + last_row[j + 1] for j in range(len(last_row) - 1)])
            row.append(1)  # Last element is also 1
        triangle.append(row)
    return triangle
num_rows = int(input())
triangle = generate_pascals_triangle(num_rows)
for row in triangle:
    print(' '.join(map(str, row)))
```
## Output:
```
    Input            Result
      5                5
                       1
                       1 1
                       1 2 1
                       1 3 3 1
                       1 4 6 4 1

```
## Result:
The program for pascal triangle was successful.

