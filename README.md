# Bank-Management-System

This project is a simple **Bank Management System** written in C that allows users to manage basic banking operations using a file-based approach. 
The system provides a text-based menu through which users can create accounts, deposit and withdraw money, and check their account balance. 
All account details are stored in a binary file (`account.dat`) to ensure data is retained between sessions.
Each account is represented using a `struct` containing the user's name, account number, and balance. 
When a user creates an account, the system initializes the balance to zero and writes the account information to the file. 
Deposits and withdrawals update the balance by reading from and writing back to the same file using file pointer positioning (`fseek`). 
Before modifying data, the program verifies that the entered account number exists.
The code includes input handling to clean up newline characters and prevent buffer issues during string input. 
File operations are used in both read (`rb`) and read/write (`rb+`) modes, and necessary checks are in place to ensure the file can be opened before performing any actions. 
This project demonstrates practical use of structures, file handling, and user interaction in C, and can serve as a foundation for more complex banking or record-keeping systems.
