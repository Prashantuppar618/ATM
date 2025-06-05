
````markdown
# 🏦 ATM Management System – Structured Enquiry Project

A C++ based **Object-Oriented ATM Management System** that simulates real-world banking functionalities such as user authentication, account management, transaction history tracking, and more. Developed as part of the *Structured Enquiry Project* for the **Object-Oriented Programming Lab (20ECSP203)** at KLE Technological University.

---

## 📘 Project Overview

The project mimics a simplified ATM system where users can:

- Authenticate using a secure PIN
- Choose between **Savings** or **Checking** accounts
- Perform actions like checking balance, depositing, withdrawing, and viewing statements
- Ensure security and validation through exception handling
- Operate in a clean, modular, and menu-driven interface

---

## ✨ Key Features

| Feature               | Description |
|-----------------------|-------------|
| 🔐 **PIN Authentication**     | Secure login using user PIN before accessing account features |
| 🏦 **Account Types**         | Supports both **Savings Account** (with min balance) and **Checking Account** (with daily limits) |
| 💰 **Deposit & Withdrawals** | Users can deposit or withdraw funds securely |
| 📊 **Balance Inquiry**       | Instantly view the current account balance |
| 🧾 **Transaction History**   | Maintains and displays all user transactions |
| 🚫 **Error Handling**        | Catches and displays helpful messages for insufficient funds or invalid amounts |
| 🧱 **Modular Classes**       | Designed with reusable and extendable OOP principles |
| 🧑‍💻 **Menu-Driven Interface**| Clear, user-friendly text-based UI with navigable choices |

---

## 🧠 Classes Used

### `BankAccount` (Abstract Base Class)
- Attributes: `accountId`, `name`, `balance`, `pin`
- Pure Virtual Function: `Instruction()`

### `SavingsAccount` & `CheckingAccount`
- Inherit from `BankAccount`
- Add `min_balance` and `daily_limit` constraints respectively

### `Transactions`
- Stores and displays individual transaction records

### `ATM`
- Handles menu display, user interaction, transaction operations

---

## 💡 How It Works

1. User chooses account type (savings/checking)
2. Enters their PIN to authenticate
3. Performs operations like:
   - Balance inquiry
   - Deposit
   - Withdraw
   - View transaction statement
4. System validates and logs all activities securely

---

## 📌 Sample Output

```text
<<<<<<<<<<<<<<<<<<<<< ATM MANAGEMENT SYSTEM >>>>>>>>>>>>>>>>>>>>>>>>>>
1. Savings
2. Checking account
Please enter your type of account: 1
Please insert your card.....
Please enter your pin: 1234

1. Check balance
2. Deposit amount
3. Withdraw amount
4. Bank statement
5. Exit
>>>>>>>>>>>>>>>Please press the choice: 1

>>>>>>This is a savings account.
Your current Balance: 10000.00
````

---

## 🗃️ Project Structure

```
├── structure_enquiry_A11.cpp        # Main C++ Source Code
├── Structure_enquiry.docx           # Design Document with Team Info and Class Diagrams
├── README.md                        # You're reading it!
```

---

## 🧪 Sample Data

```cpp
SavingsAccount("SBI@1548000048", "Mary", 10000.00, 1234, 1000.00);
CheckingAccount("SBI@1548000049", "Jeson", 11000.00, 4567, 40000.00);
```

---



## 🧾 License

MIT License – Free to use with credit to the authors.

---

## 🛠️ Future Enhancements

* 🔐 Encrypted storage for PINs
* 🌐 Web-based ATM simulation
* 📄 Persistent file/database storage
* 🧪 Automated test suites for transaction logic

---

## 🙏 Acknowledgments

* C++ Standard Library
* KLE Technological University
* Our Faculty Guide

---


