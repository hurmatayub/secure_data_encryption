# 🔒 Secure Data Vault

[Access the live app here](https://secure-data-vault-5.streamlit.app/)

## Overview

The **Secure Data Vault** is a web application built using Streamlit, Python, and the `cryptography` library, designed to securely store and retrieve sensitive data. It uses encryption and hashing techniques to ensure the safety and privacy of the stored information.

## Features

- **Store Data**: Users can securely store their data by encrypting it with a custom passkey. The data is saved in an encrypted format, ensuring privacy.
- **Retrieve Data**: Users can retrieve their stored data by providing the correct passkey. The application decrypts the data and presents it to the user.
- **User Authentication**: The app includes a login page that uses a master password to ensure only authorized access to the data.
- **Encryption and Decryption**: The data is encrypted using the `cryptography.fernet` method, ensuring robust data protection.

## Technologies Used

- **Streamlit**: For creating the web interface.
- **Python**: Main programming language.
- **Cryptography**: To encrypt and decrypt data.
- **Hashlib**: To hash the passkeys for storage and validation.



## How to Use

1. **Store Data**: 
    - Enter a unique username, a passkey (password), and the data you wish to store.
    - Click on the **Encrypt & Save** button to securely store your data.

2. **Retrieve Data**:
    - Enter your username and passkey.
    - Click **Decrypt** to retrieve and view your stored data.

3. **Login**:
    - Enter the **master password** (`admin123`) to reauthorize yourself if necessary.

## Security

- The app uses **Fernet encryption** to securely encrypt and decrypt data.
- The passkeys are hashed using **SHA-256** for secure storage and validation.
- If too many incorrect passkey attempts are made, access is locked, and you are redirected to the login page.

