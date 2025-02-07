# Python File Encryption Scripts

Python scripts for file encryption/decryption on Linode cloud platform. Based on tutorial: [Encryption Tutorial](https://www.youtube.com/watch?v=UtMMjXOlRQc)

## Description
This project implements file encryption and decryption scripts designed to work with cloud storage on the Linode platform. The scripts provide secure file handling and demonstrate basic cryptographic principles.

## Technologies
- Python 3.x 
- Cryptography library
- Linode platform
- Linux commands

## Features
- File encryption using symmetric key algorithms
- Secure key generation and storage
- File decryption capabilities
- Cloud storage integration
- Batch processing support
- Command-line interface

## Requirements
- Python 3.6+
- cryptography package
- Linode account and API access
- Linux/Unix environment

## Installation
1. Clone repository:
2. pip install cryptography
3. pip install linode-api4
4. export LINODE_TOKEN='your_api_token'

## Usage
To encrypt a file:
bashCopypython encrypt.py <input_file> <output_file>
To decrypt a file:
bashCopypython decrypt.py <encrypted_file> <output_file>

## Security Considerations

Store encryption keys securely
Use strong passwords
Keep encrypted backups
Don't share keys in plaintext
Regular key rotation recommended

## Project Structure
Copy├── src/
│   ├── encrypt.py
│   ├── decrypt.py
│   └── utils.py
├── tests/
├── requirements.txt
└── README.md

## Credits
Based on the tutorial by NetworkChuck
