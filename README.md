# 🏦 Simple ATM Simulator in C

This is my first project developed in C for the **"Basics of Programming"** university course. It is a console-based ATM simulator that features two distinct operational modes: an Employee (Admin) panel and a Customer panel. The project strictly validates user inputs and uses binary file I/O to save state across sessions.

## ✨ Features

### 👨‍💼 Employee (Admin) Panel
* **Create Accounts:** Register new customers with complete details (Name, ID, Phone, Card Number, Initial Balance, Password).
* **Edit Accounts:** Modify existing customer details securely.
* **Rich Customer Lookup:** Automatically search and display the customer with the highest account balance.
* **Bank Assets:** Calculate and show the total balance of all accounts combined.
* **Customer List:** Display a list of all registered customers and their information.

### 💳 Customer Panel
* **Account Balance:** Check current available funds.
* **Cash Transfer:** Transfer money to other valid cardholders securely.
* **Cash Withdrawal:** Withdraw money with real-time balance updates.
* **Password Management:** Change the 4-digit account PIN.

### ⚙️ System & Security
* **Data Persistence:** All customer data is securely saved to and loaded from a `customer.bin` file.
* **Input Validation:** Strict format checking for IDs (10 digits), Phone numbers (11 digits, starts with 09), Card numbers (16 digits), and PINs (4 digits).
* **Interactive UI:** Colored console outputs (using ANSI escape codes) for a better user experience.

## 📂 Project Structure

The project is structured modularly for better readability and maintenance:
* `main.c`: The entry point of the application.
* `menu.h`: Handles the main selection interface.
* `employee.h`: Contains all functions and logic for the Admin panel.
* `customer.h`: Contains all functions and logic for the Customer operations.

## 🚀 How to Run

### Prerequisites
* A C compiler (e.g., GCC).
* **Note:** This project uses `conio.h` and `system("cls")`, which means it is designed to run natively on **Windows** environments.

### Compilation
Open your terminal or command prompt in the project directory and compile the files:
```bash
gcc main.c -o atm_simulator
