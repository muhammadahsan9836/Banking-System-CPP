# 🏦 Banking System Console App – C++ Data Structures Project

A complete console-based banking system demonstrating **custom linked lists**, **OOP**, **PIN encryption**, **multi‑level access control**, and **file persistence**. Built with pure C++ (C++98 compatible) – no external libraries.

## ✨ Features

### 🔐 Multi‑Level Access
- **Admin** (master PIN: `ADMIN999`) – manage all accounts
- **Customer** (login with account number + PIN) – personal banking

### 👤 Customer Operations
- Deposit / Withdraw money
- Transfer funds to any other account
- View transaction history (deposits, withdrawals, transfers)
- Change own PIN securely

### 🛠️ Admin Operations
- Create new account (auto‑generates unique account number, CNIC must be unique)
- Delete any account
- List all accounts (formatted table)
- View transaction history of any account
- Search account by CNIC

### 🧠 Technical Highlights
- **Custom singly linked list** (`LinkedList<T>`) – no STL containers
- **XOR encryption** for PIN storage (simple yet demonstrates security awareness)
- **Transaction logging** – each account tracks its own history
- **File persistence** – all accounts saved to `data/accounts.txt`, reloaded on startup
- **Input validation** – handles wrong data types, negative amounts, insufficient balance
- **C++98 compatible** – runs on older compilers (Dev‑C++, MinGW)

## 📸 Screenshots

> *Add your own console screenshots here after running the program.*  
> Example:  
> ![Admin Menu](screenshots/admin-menu.png)  
> ![Transaction History](screenshots/history.png)

## 🚀 How to Compile and Run

### Prerequisites
- Windows PC with **Dev‑C++** (or any C++98 compiler like MinGW)
- No extra libraries required

### Steps
1. **Clone or download** this repository.
2. Open the project folder and **create a subfolder named `data`** (this is where accounts are saved).
3. Open `main.cpp` in Dev‑C++ (or your compiler).
4. **Compile** (F11 in Dev‑C++) – the code is self‑contained, no extra headers needed.
5. **Run** the executable.

### First Run
- No accounts exist initially. Log in as **Admin** (`ADMIN999`) and create your first customer account.
- After creating an account, you can log out and log in as that customer.

## 🧪 Example Usage
=== BANKING SYSTEM ===

Admin Login

Customer Login

Exit
Choice: 1

Enter Admin Master PIN: ADMIN999

--- ADMIN MENU ---

Create Account

Delete Account

List All Accounts

View Account History

Search by CNIC

Logout
Choice: 1

CNIC: 12345-6789012-3
Full Name: Ahsan
PIN: 1234
Initial Deposit: 5000
Account created: ACC12345
Then log in as customer, deposit, withdraw, transfer, etc.

## 🗂️ File Structure
BankingSystem/
├── main.cpp (complete source code)
├── data/ (created automatically; stores accounts.txt)
│ └── accounts.txt (saved accounts – each line: accNo|CNIC|name|encryptedPIN|balance)
└── README.md


## 📚 What I Learned / Demonstrated

- Implementing **custom linked list** from scratch (node structure, dynamic memory, traversals)
- **Encapsulation** and **object‑oriented design**
- **File I/O** – saving/loading account data in a human‑readable format
- **Encryption basics** – XOR cipher for PINs
- **Robust input handling** – avoiding crashes on bad user input
- **Separation of concerns** – menus, business logic, data storage in one coherent file

## 🔮 Future Improvements (Ideas)

- Add transaction persistence (save each transaction to a separate file)
- Sort accounts by balance using a sorting algorithm on linked list
- Add interest calculation for savings accounts (polymorphism)
- Convert to a GUI using Qt or a web‑based frontend

## 📄 License

Feel free to use, modify, and share this project for learning purposes.

## 👤 Author

**Muhammad Ahsan**  
[GitHub Profile Link – https://github.com/muhammadahsan9836]  
[LinkedIn Link – www.linkedin.com/in/muhammad-ahsan-155822323]
