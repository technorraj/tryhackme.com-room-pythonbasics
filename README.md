
# 🐍 TryHackMe: Python Basics – Walkthrough

This document contains a complete walkthrough of the **Python Basics** room on TryHackMe. It's designed for beginners and covers essential Python concepts like printing, arithmetic, variables, conditionals, loops, functions, and file handling.

---

## 📌 Basic Printing

To begin with, we print a simple string to the console:

```python
print("Hello World")
```

**Flag:** `THM{PRINT_STATEMENTS}`

---

## ➗ Arithmetic Operations

Performing different arithmetic operations in Python:

```python
# Addition
print(21 + 43)  # 64

# Subtraction
print(142 - 52)  # 90

# Multiplication
print(10 * 342)  # 3420

# Exponentiation (5 squared)
print(5**2)  # 25
```

**Flags:**
- Addition: `THM{ADDITI0N}`
- Subtraction: `THM{SUBTRCT}`
- Multiplication: `THM{MULTIPLICATION_PYTHON}`
- Exponentiation: `THM{EXP0N3NT_POWER}`

---

## 🧮 Variables

We assign and update variables:

```python
height = 200
height = height + 50
print(height)  # 250
```

**Flag:** `THM{VARIABL3S}`

---

## 🚚 Conditional Logic – Shipping Calculator

Simple conditional logic based on cost:

```python
customer_basket_cost = 34
customer_basket_weight = 44

if customer_basket_cost > 100:
    print("free shipping")
else:
    shipping = 1.20 * customer_basket_weight
    total = customer_basket_cost + shipping
    print(total)  # 86.8
```

**Flag:** `THM{IF_STATEMENT_SHOPPING}`

If we increase the basket cost to trigger free shipping:

```python
customer_basket_cost = 101
customer_basket_weight = 44

if customer_basket_cost > 100:
    print(customer_basket_cost)  # 101
else:
    shipping = 1.20 * customer_basket_weight
    total = customer_basket_cost + shipping
    print(total)
```

**Flag:** `THM{MY_FIRST_APP}`

---

## 🔁 Loops

Loop from 0 to 50 using a `for` loop:

```python
for i in range(51):
    print(i)
```

**Flag:** `THM{L00PS_WHILE_FOR}`

---

## 💰 Functions & Conditions – Bitcoin Alert

Define a function and use it to trigger alerts based on value:

```python
def bitcoinToUSD(bitcoin_amount, bitcoin_value_usd):
    total = bitcoin_amount * bitcoin_value_usd
    return total

flag = bitcoinToUSD(1.2, 4000)

if flag < 30000:
    print("Alert!!!")
elif flag == 30000:
    print("It's worth 30k bro")
else:
    print("It's worth more than 30k bro")
```

**Flag:** `THM{BITC0IN_INVESTOR}`

---

## 📂 File Handling

Read content from a file:

```python
file = open("flag.txt", "r")
print(file.read())
```

**Flag:** `THM{F1LE_R3AD}`

---

## ✅ Summary

This TryHackMe room introduced foundational Python programming through real-world-style examples. These concepts are essential for automation, scripting, and cybersecurity-related tasks.

> Completed and documented by [technor_raj](https://technorraj.github.io/)  
> Room: [TryHackMe - Python Basics](https://tryhackme.com)
