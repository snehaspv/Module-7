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

```
def series(x, n):
    if n == 0:
        return 1
    else:
        return (x**n / n) + series(x, n - 1)
x = int(input())
n = int(input())
print(series(x, n))
```


## OUTPUT
<img width="434" height="179" alt="image" src="https://github.com/user-attachments/assets/6f60e055-5e76-45f5-b590-bc2b39a5d658" />

## RESULT
Thus, the Python program to evaluate a Taylor Series using recursion is executed successfully.
