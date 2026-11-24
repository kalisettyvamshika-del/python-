# 🏥 Hospital Billing and Patient Classification

## 📌 Project Overview

The Hospital Billing and Patient Classification system is a Python-based application designed to calculate hospital bills based on consultation fees, diagnostic charges, and treatment costs.

The program applies concessions according to patient categories and classifies patients based on their final billing amount.

## 🎯 Objectives

- Calculate the total hospital bill.
- Apply discounts for eligible patients.
- Calculate the final payable amount.
- Classify patients based on their billing amount.
- Understand basic Python programming concepts.

## 🛠️ Technologies Used

- **Programming Language:** Python 3
- **Editor:** VS Code / IDLE
- **Platform:** Windows / Linux

## 📚 Python Concepts Used

- Variables and Data Types
- User Input and Output
- Arithmetic Operators
- Conditional Statements (`if`, `else`)
- String Methods (`lower()`)

## ⚙️ Assumptions

1. Senior citizens receive a 10% discount.
2. General patients receive no discount.
3. Bills above ₹10,000 are classified as High Bills.
4. Bills of ₹10,000 or below are classified as Normal Bills.
5. All billing amounts must be positive.

## 💻 Source Code

```python
# Hospital Billing and Patient Classification

name = input("Enter patient name: ")

category = input("Enter patient category: ")

consultation = float(input("Enter consultation fee: "))

diagnostic = float(input("Enter diagnostic charges: "))

treatment = float(input("Enter treatment charges: "))

# Calculate total bill
total = consultation + diagnostic + treatment

# Calculate discount
if category.lower() == "senior":
    discount = total * 0.10
else:
    discount = 0

# Calculate final bill
final_bill = total - discount

# Patient classification
if final_bill > 10000:
    classification = "High Bill"
else:
    classification = "Normal Bill"

# Display bill
print("\n----- HOSPITAL BILL -----")

print("Patient Name:", name)
print("Patient Category:", category)
print("Total Amount:", total)
print("Discount:", discount)
print("Final Bill:", final_bill)
print("Classification:", classification)
```

## 🧪 Sample Input

```text
Enter patient name: Ravi
Enter patient category: senior
Enter consultation fee: 500
Enter diagnostic charges: 1500
Enter treatment charges: 8000
```

## 📤 Sample Output

```text
----- HOSPITAL BILL -----

Patient Name: Ravi
Patient Category: senior
Total Amount: 10000.0
Discount: 1000.0
Final Bill: 9000.0
Classification: Normal Bill
```

## 📊 Test Cases

| Test Case | Category | Total Amount | Discount | Final Amount |
|---|---|---:|---:|---:|
| 1 | Senior | ₹10,000 | ₹1,000 | ₹9,000 |
| 2 | General | ₹12,000 | ₹0 | ₹12,000 |
| 3 | Senior | ₹5,000 | ₹500 | ₹4,500 |

## 🔄 Working Process

1. Enter patient information.
2. Enter consultation, diagnostic, and treatment charges.
3. Calculate the total bill.
4. Check the patient category.
5. Apply the eligible discount.
6. Calculate the final payable amount.
7. Display the billing classification.

## 🏁 Conclusion

This project demonstrates how Python can be used to automate hospital billing calculations. It provides practical understanding of variables, data types, arithmetic operators, and conditional statements.

## 👩‍💻 Project Details

**Project Name:** Hospital Billing and Patient Classification

**Case Study Number:** 3

**Project Type:** Python Activity-Based Learning

**Programming Language:** Python 3
