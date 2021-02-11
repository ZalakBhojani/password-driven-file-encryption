# Password-Driven-File-encryption

The script uses cryptography package for password driven file encryption-decryption. 

## Getting Started

The user can provide a password that would in turn used to generate a key. The key is generated using SHA256 hash algorithm. The key can be used to further encrypt the file. The encrypted file can then be shared among users, however without the key or password along with the script the user cannot decrypt the content of the file. It is suggested to not share the key.

### Prerequisites

Python3, pip

### Installing

Clone/Download the repository and run the following command using the terminal

```
pip install -r requirements.txt
```

## Running the script

The following command helps the user to get familiar with the script

```
python3 crypt.py -h
```
which outputs 

```
File Encryptor Script

positional arguments:
  file                File to encrypt/decrypt

optional arguments:
  -h, --help          show this help message and exit
  -g, --generate-key  Whether to generate a new key or use existing
  -e, --encrypt       Whether to encrypt the file, only -e or -d can be
                      specified.
  -d, --decrypt       Whether to decrypt the file, only -e or -d can be
                      specified.
```

Make sure to change the password at line 14 according to the usage

## Built With

* cryptography - (https://cryptography.io/en/latest/) - package for safe and secure implementation of encryption and decryption of files
* argparse - (https://docs.python.org/3/library/argparse.html) - library for user - friendly command-line interface
* base64 - (https://docs.python.org/3/library/base64.html) - library for converting the byte like object key to urlsafe encoded byte key
* os - (https://docs.python.org/3/library/os.html) - module for file read and write operations

The script was made as a part of submissions for 2UCL602 - Cryptography and System Security lab
