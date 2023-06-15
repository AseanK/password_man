# Password Manager
<img src='passman.gif'>

## About
This is a simple password manager application built with Python. It provides a graphical user interface (GUI) using the tkinter module, allowing users to manage their passwords securely. The application offers the following features:

## Features
**GUI Manager**: The password manager has a user-friendly graphical interface, making it easy for users to navigate and interact with the application.

**Password Generation**: Users can either enter their own passwords or generate strong passwords using the built-in password generator. The generated passwords adhere to the following criteria:
- Length: 12 to 18 characters
- Letters: 8 to 10 letters (both uppercase and lowercase)
- Numbers: 2 to 4 numbers
- Symbols: 2 to 4 symbols

**Key Generation**: The password manager generates a key using the Fernet module for encryption and decryption. Users have the flexibility to specify the path where they want to store the key.

**Key Management**: It is crucial for users to safely keep their encryption key since it is used to encrypt and decrypt their passwords. Loss of the key may result in irreversible data loss. A reminder is provided to users to ensure they keep the key in a secure location.

**Password Encryption**: The passwords are encrypted using the Fernet encryption algorithm. The Fernet module provides a symmetric encryption method, which means the same key is used for both encryption and decryption.

**JSON File Storage**: The encrypted passwords are stored as a JSON file, ensuring easy accessibility and maintainability. Each website entry includes the website name, associated email address, and the encrypted password.

## Getting Started
**To use the password manager, follow these steps:**

### Step 1
- Clone the repository using either of the following commands: 
```bash
git clone git@github.com:AseanK/python-tools-and-games.git
```
or
```bash
git clone https://github.com/AseanK/python-tools-and-games.git
```

### Step 2
- After cloning the repository, navigate to the project directory:
```bash
cd "<Name_of_the_folder>"
```

### step 3
Install the required dependencies by running the following command:
```bash
pip install -r requirements.txt
```

### Step 4
Run the application using the following command:
```bash
python main.py
```
The graphical user interface will be displayed, allowing you to enter and manage your passwords securely.

**Note: It is essential to keep your encryption key in a safe and secure location. Losing the key may result in permanent data loss.**

## Contributing
Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue on the GitHub repository.

## Acknowledgments
The password manager utilizes the tkinter module for the graphical user interface.
Encryption and decryption are performed using the cryptography library's Fernet module.
The project was inspired by the need for secure password management and aims to provide a simple and intuitive solution.
