# Encryption-Decryption Project 


**Encryption-Decryption** is a text encryption and decryption application that allows users to securely encrypt and decrypt messages using both AES (Advanced Encryption Standard) and RSA (Rivest–Shamir–Adleman) algorithms. The application provides a user-friendly graphical interface using Tkinter, where users can input their plaintext messages, enter a key, and encrypt or decrypt them.

## Features

- **AES Encryption**: Uses the AES encryption standard to encrypt and decrypt messages.
- **RSA Key Generation**: Generates RSA public and private keys for encryption and decryption.
- **Symmetric and Asymmetric Encryption**: Both AES (symmetric) and RSA (asymmetric) encryption are supported.
- **Graphical User Interface (GUI)**: Simple and intuitive interface for encryption and decryption operations.

## Tools and Technologies

- **Programming Language**: Python
- **Cryptographic Libraries**: 
  - PyCryptodome (for AES and RSA encryption/decryption)
- **GUI Framework**: Tkinter (for building the application interface)

## Installation

Follow these steps to install the required packages and run the application:

### 1. Install Python

Make sure Python is installed on your system. You can download Python from [here](https://www.python.org/downloads/).

### 2. Install the Required Packages

Install the dependencies using `pip`:

```bash
pip install pycryptodome
```

Note: **Tkinter** comes pre-installed with Python. If you are using a Python distribution where it's not installed by default, you may need to install it separately.

### 3. Running the Application

Once the dependencies are installed, you can run the application:

```bash
python secure_text_app.py
```

## How It Works

### AES Encryption & Decryption

1. **AES Encryption**: The plaintext is encrypted using a 16-byte key (either padded or truncated to 16 bytes). The encrypted message is returned in base64 format.
2. **AES Decryption**: The encrypted message is decrypted using the same 16-byte key. If the key is incorrect or the ciphertext is tampered with, an error will be raised.

### RSA Key Generation

1. **RSA Key Generation**: RSA keys are generated using a key size of 2048 bits. The generated keys can be used for RSA encryption and decryption.
2. **RSA Encryption**: The plaintext is encrypted using the public RSA key, and the ciphertext is returned in base64 format.
3. **RSA Decryption**: The ciphertext is decrypted using the private RSA key.

### Graphical User Interface (GUI)

- **Key Input**: Enter the encryption/decryption key (must be a 16-byte string for AES).
- **Plaintext**: Enter the message you want to encrypt.
- **Ciphertext**: View the encrypted message after encryption.
- **Encrypt Button**: Encrypt the plaintext using the specified key.
- **Decrypt Button**: Decrypt the ciphertext using the specified key.

## Usage

1. **AES Encryption**: 
   - Enter the message in the "Plaintext" field.
   - Enter the key (16 bytes) in the "Key" field.
   - Click the "Encrypt" button. The ciphertext will appear in the "Ciphertext" field.
   
2. **AES Decryption**: 
   - Enter the encrypted message in the "Ciphertext" field.
   - Enter the key (16 bytes) in the "Key" field.
   - Click the "Decrypt" button. The plaintext will appear in the "Plaintext" field.

## Example

1. **AES Encryption Example**:

    - Plaintext: "Hello, world!"
    - Key: "mysecretkey1234"
    - Ciphertext: `Encrypted message`

2. **AES Decryption Example**:

    - Ciphertext: `Encrypted message`
    - Key: "mysecretkey1234"
    - Plaintext: "Hello, world!"

## Future Improvements

- **RSA Encryption and Decryption**: Add GUI support to allow users to encrypt and decrypt using RSA keys.
- **Enhanced User Interface**: Provide a better layout and add more features like file encryption/decryption.
- **Additional Cryptographic Algorithms**: Support for more algorithms like DES, 3DES, etc.

