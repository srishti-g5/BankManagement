# Banking System Project Readme

## Overview
This Java-based Banking System project is designed to operate basic banking operations such as user registration, account management, and transactions. The project utilizes MySQL for database and includes classes for managing users (`User`), accounts (`Accounts`), and account transactions (`AccountManager`).

## Features
1. **User Registration and Login:**
   - Users can register with their full name, email, and password.
   - Existing users can log in with their email and password.

2. **Account Management:**
   - Users can open new bank accounts if they don't have one.
   - Each account has a unique account number, associated with the user's email.
   - Users can check their account balance, credit money, debit money, and transfer money to other accounts.

3. **Security Features:**
   - User passwords are stored securely in the database (considered for future implementations).
   - Security pins are used for account transactions, providing an additional layer of security.

4. **Database Integration:**
   - The project uses MySQL for database storage.
   - The schema includes tables for user information (`User`) and account details (`Accounts`).

## Project Structure
1. **Main Class (`BankingSystem`):**
   - Acts as the entry point of the program.
   - Manages the overall flow of the banking system, including user registration, login, and account operations.

2. **User Class (`User`):**
   - Handles user-related operations such as registration, login, and checking user existence.

3. **Accounts Class (`Accounts`):**
   - Manages account-related operations, including opening new accounts, retrieving account numbers, and checking account existence.

4. **AccountManager Class (`AccountManager`):**
   - Manages financial transactions such as crediting, debiting, transferring money, and checking account balances.

## Database Schema
The project assumes the existence of a MySQL database named `banking_system` with the following tables:
1. **User Table:**
   - `full_name`: Full name of the user.
   - `email`: User's email address.
   - `password`: User's password (to be enhanced with secure password storage).

2. **Accounts Table:**
   - `account_number`: Unique account number for each account.
   - `full_name`: Full name associated with the account.
   - `email`: Email associated with the account.
   - `balance`: Current account balance.
   - `security_pin`: Security pin for account transactions.

## Usage
1. **Database Setup:**
   - Set up a MySQL database named `banking_system`.
   - Update the database connection details in the `BankingSystem` class.

2. **Run the Program:**
   - Execute the `BankingSystem` class to start the program.
   - Follow the on-screen instructions to register, log in, and perform various banking operations.


## Future Enhancements
1. **Password Encryption:**
   - Enhance security by implementing password encryption techniques.

2. **UI Enhancement:**
   - Consider implementing a graphical user interface (GUI) for a more user-friendly experience.

## Acknowledgments
This project is a basic simulation and is meant for educational purposes.
