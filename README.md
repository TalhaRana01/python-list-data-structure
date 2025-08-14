# 📃 List - Data Structure

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python&logoColor=yellow)
![GitHub](https://img.shields.io/badge/GitHub-Repo-black?logo=github)
[![Email](https://img.shields.io/badge/Emailmtalharna093@gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:TalhaRana01@gmail.com)

A **list** in Python is an **ordered collection of values**.  
Lists are **mutable**, allow **duplicate elements**, and can be accessed using **forward** or **backward indexing**.

---

## 📑 Table of Contents
1. [Key Features](#-key-features)
2. [Example: List Operations](#-example-list-operations)
3. [Tips & Best Practices](#-tips--best-practices)
4. [Output Examples](#-output-examples)
5. [Contact](#-contact)
6. [License](#-license)

---

## 🔹 Key Features

- **Symbol:** `[ ]`  
- **Forward Index:** 0, 1, 2, 3, ...  
- **Backward Index:** -1, -2, -3, ...  
- **Mutable:** Yes  
- **Duplicates Allowed:** Yes  

---

## 💻 Example: List Operations

```python
# 1️⃣ Creating lists
marks = [90, 80, 60, 20, 40, 70, 100, 50]
marks1 = [50, 60, 40, 80, 90, 30, 20]

print("Marks =", marks)  # Marks = [90, 80, 60, 20, 40, 70, 100, 50]

# 2️⃣ Accessing elements
marks[0]    # First element: 90
marks[1]    # Second element: 80
marks[7]    # Last element: 50
# marks[8]  # ❌ Error: list index out of range
print(len(marks))  # Length of list: 8

# 3️⃣ Slicing lists
marks[1:4]      # [80, 60, 20] (index 4 not included)
marks[0:5]      # [90, 80, 60, 20, 40]
marks1[1:2]     # [60]
marks1[2:3]     # [40]
marks1[3:6]     # [80, 90, 30]
marks1[4:6]     # [90, 30]
marks1[4:6:2]   # [90] (step = 2)
marks1[2:6:2]   # [40, 90] (step = 2)
marks1[0:6]     # [50, 60, 40, 80, 90, 30]
marks1[0:6:2]   # [50, 40, 90]

# 4️⃣ Negative indexing
marks1[-1]      # 20
marks1[-2]      # 30
marks1[-5]      # 60
marks1[-7]      # 50
marks1[-7:-1:2] # [50, 40, 90]

# 5️⃣ Loop through list using for loop
for mark in marks1:
    print(mark)  # Prints all elements

# 6️⃣ Loop using while
mark = 0
while mark < len(marks1):
    print(marks1[mark])
    mark += 1

# 7️⃣ Conditional checks using for loop
for mark in marks1:
    if mark > 50:
        print(f"{mark}: ✅ Passed")
    else:
        print(f"{mark}: ❌ Failed")

# 8️⃣ Conditional checks using while loop
mark = 0
while mark < len(marks1):
    if marks1[mark] > 50:
        print(marks1[mark], "✅ Passed")
    else:
        print(marks1[mark], "❌ Failed")
    mark += 1
