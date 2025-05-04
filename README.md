# 🏦 Bank Management System in C

This is a mini-project developed in C that simulates core banking operations via a command-line interface. It supports creating multiple user accounts, handling transactions (deposit, withdraw, transfer), and managing data persistence through file handling. The project demonstrates structured programming, use of pointers, structures, and file I/O.

---

## 🎯 Features

- ✅ Create new accounts with unique account numbers
- 💰 Deposit and withdraw funds
- 🔁 Transfer money between accounts
- 📊 View account balance
- 📜 Display transaction history (last 5 transactions per account)
- 🔍 Search for specific accounts
- 📂 Display all account details
- 💾 Save and load data from files
- ⏳ Persistent data between sessions

---

## 🧱 Tech Stack

- Language: **C**
- Data Storage: **File Handling (Text/Binary)**
- Data Structures: **Structure Pointers**, **Single Linked List (SLL)**

---

## 🗃️ Data Structure Design

Each account contains:
- `account_number`
- `account_name`
- `account_balance`
- `contact_number`
- `transaction_count`
- `transactions[]` – An array of transaction structures:
  - `transaction_id` (auto-incremented `uint32_t`)
  - `transaction_type` (enum: DEPOSIT, WITHDRAW)

---

## 🧑‍💻 Menu Interface

When the app runs, it presents the following menu:

```
------------------MENU---------------------------
c/C:     Create account
h/H:     View last 5 transactions
w/W:     Withdraw amount
d/D:     Deposit amount
b/B:     Balance enquiry
t/T:     Transfer money
e/E:     Display all accounts
s/S:     Save all account data
f/F:     Find specific account
q/Q:     Quit
```

---

## 🛠️ Build & Run

```bash
make         # Compiles the project
./bank       # Runs the banking system
```

> 💡 Use `make clean` to remove compiled files.

---

## 📁 Project Structure

- `main.c` – Entry point and menu handling
- `account.c` – Create, search, display accounts
- `transaction.c` – Deposit, withdraw, transfer
- `fileops.c` – Save/load account data
- `makefile` – To build the project
- `README.md` – Project documentation
- `accounts.txt` – Persistent data storage

---

## 📌 Key Concepts Practiced

- Modular programming in C
- File handling for data persistence
- Linked list implementation using pointers
- Use of `typedef`, `enum`, and `struct`

---

## 🚀 Future Improvements

- Login/password protection for accounts
- Admin and user modes
- Interest calculation logic
- Enhanced transaction filtering and reports

---

## 📚 License

This project is for academic and learning purposes. Free to use and modify.
