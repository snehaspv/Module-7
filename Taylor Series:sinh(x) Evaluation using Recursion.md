# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:

```
def fact(n):
    if n <= 1:
        return 1
    else:
        return n * fact(n - 1)
def sinh(x, n):
    if n == 0:
        return x
    else:
        return (pow(x, 2 * n + 1) / fact(2 * n + 1)) + sinh(x, n - 1)
x = float(input())
n = int(input())
print("sinh(", x, ") =", sinh(x, n))
```


## OUTPUT
<img width="398" height="157" alt="image" src="https://github.com/user-attachments/assets/70f11685-4d77-4cb5-8b39-283bbbd860fa" />

## RESULT
Thus, the Python program to evaluate the value of sinh(x) for n terms using recursion is executed successfully.
