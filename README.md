# File encryption exercise

My Python encryption and decryption exercise, based on [NetworkChuck’s tutorial](https://www.youtube.com/watch?v=UtMMjXOlRQc).

The two scripts use `cryptography.fernet` to encrypt and decrypt files in the current directory. They do not accept input/output filename arguments and do not call the Linode API.

## Read before running

`encrypt.py` generates a key, writes it to `thekey.key`, and overwrites the files it selects in the current directory. Its exclusion list still refers to `voldemort.py`, the tutorial’s filename, so it can also select the scripts themselves.

`decrypt.py` reads `thekey.key` and attempts to decrypt the selected files in place. Decryption depends on keeping the original key.

Use disposable copies in a separate test folder if you want to study the behaviour. This repo is a learning exercise, not a backup or file-protection tool.

## Dependency

Python and the `cryptography` package.
