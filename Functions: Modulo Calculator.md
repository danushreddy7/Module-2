# Functions in Python: Modulo Calculator

## 🎯 Aim:
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm:
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program:
```
def get_modulo(a, b):
    return a % b
num1 = 17
num2 = 5
result = get_modulo(num1, num2)
print(f"The result of {num1} % {num2} is {result}")
```
## Output:
```
  Input            Result

   17
               The result of 17 % 5 is 2
   5
```
## Result:
The program to return two values modulo is successful.
