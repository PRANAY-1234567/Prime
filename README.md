📘 README — Prime Numbers in Range (Python)

📌 Description

This Python program prints all **Prime Numbers** between a given range.

In this code, the range is from **1 to 20**.

---

## 🔢 What is a Prime Number?

A **Prime Number** is a number that:

* Is **greater than 1**
* Has **only 2 divisors** → 1 and itself

👉 Examples:
2, 3, 5, 7, 11, 13, 17, 19

---

## ⚙️ Code

```python
start = 1
end = 20

for num in range(start, end + 1):
    if num > 1:
        for i in range(2, num):
            if num % i == 0:
                break
        else:
            print(num)
```

---

## 🧠 Step-by-Step Explanation (Very Simple)

### 1️⃣ Define range

```python
start = 1
end = 20
```

We want to check numbers between **1 and 20**.

---

### 2️⃣ Loop through each number

```python
for num in range(start, end + 1):
```

This checks every number one by one.

---

### 3️⃣ Prime numbers must be greater than 1

```python
if num > 1:
```

---

### 4️⃣ Check divisibility

```python
for i in range(2, num):
```

We check if the number can be divided by any value between **2 and num-1**.

---

### 5️⃣ If divisible → not prime

```python
if num % i == 0:
    break
```

If remainder = 0 → number is NOT prime.

---

### 6️⃣ If loop never breaks → it is prime

```python
else:
    print(num)
```

This special `else` belongs to the **for loop**, not the `if`.

It runs only when the loop completes fully.

---

## ▶️ Output

```
2
3
5
7
11
13
17
19
```

---

## 💡 Key Concepts Learned

* Nested loops
* Range function
* Modulus operator `%`
* Prime number logic
* For-else concept in Python

---

## 🚀 Real-World Use

This logic is used in:

* Cryptography
* Security systems
* Mathematical calculations
* Coding interviews

---

## ⭐ Simple Trick to Remember

👉 Prime number = **Only divisible by 1 and itself**

---
👨‍💻 Author
Pranay Jadhao

<img width="660" height="880" alt="image" src="https://github.com/user-attachments/assets/6874088e-8c6c-4602-8e6f-ba2c667246e9" />

