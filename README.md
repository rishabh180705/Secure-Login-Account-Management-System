# Secure-Login-Account-Management-System
Overview
The Secure Login and Account Management System is a C++ application that provides a secure way for users to create, log in, and manage their accounts. It ensures proper authentication and secure handling of user data by implementing various security mechanisms, such as password hashing, account validation, and file-based data storage.

The system provides a command-line interface (CLI) where users can:

Create a new account
Log in to an existing account
Change their password
Delete their account
View account details
Features
Account Creation:

Users can create new accounts by providing a username and password. Passwords are hashed for security.
Secure Login:

Users can log in using their username and password. The system compares the hashed password for authentication.
Password Hashing:

Passwords are hashed using algorithms such as SHA-256 to ensure they are stored securely. Plain-text passwords are never saved.
Password Change:

Users can securely update their passwords. The new password is hashed and updated in the system.
Account Deletion:

Users can delete their accounts if needed, and all associated data is removed from the system.
File-Based Data Storage:

User account information is stored in a file using encryption and hashing to ensure security and integrity.
Validation:

The system checks for common vulnerabilities, such as weak passwords and improper usernames, during account creation.
How It Works
The system operates through a simple CLI that prompts users for input, handles authentication, and manages account data. It works as follows:

Account Creation Process:

The user provides a username and password.
The password is hashed, and the username along with the hashed password is stored in a file (e.g., accounts.txt).
Login Process:

The user enters their username and password.
The system retrieves the stored hashed password and compares it to the hash of the entered password. If they match, the login is successful.
Password Change:

Once logged in, users can choose to update their password. The new password is hashed and replaces the old hashed password.
Account Deletion:

Upon successful login, the user can opt to delete their account, which will remove their data from the file.
License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code.
