# Cryptographic Project using GPG

## Overview

This project demonstrates the practical implementation of cryptographic techniques using GNU Privacy Guard (GPG) on Ubuntu Linux.

## Features

- RSA key pair generation
- Public key export
- File encryption
- File decryption
- Digital signature creation
- Signature verification
- SHA-256 hashing
- Secure communication workflow

## Files

- report.txt
- report.enc
- decrypted_report.txt
- message.txt
- message.txt.asc
- message.txt.gpg
- publickey.asc
- report_hash.txt
- backup.enc
- restored_backup.txt

## Technologies Used

- Ubuntu Linux
- GnuPG (GPG)
- SHA-256
- Bash Terminal

## Commands Used

Generate Keys

```bash
gpg --full-generate-key
```

List Keys

```bash
gpg --list-keys
```

Export Public Key

```bash
gpg --armor --export your_email@example.com > publickey.asc
```

Encrypt File

```bash
gpg --encrypt --recipient your_email@example.com report.txt
```

Decrypt File

```bash
gpg --decrypt report.enc > decrypted_report.txt
```

Create Digital Signature

```bash
gpg --clearsign message.txt
```

Verify Signature

```bash
gpg --verify message.txt.asc
```

Generate SHA-256 Hash

```bash
sha256sum report.txt > report_hash.txt
```

## Skills Demonstrated

- Public Key Cryptography
- Digital Signatures
- Secure File Encryption
- Hash Functions
- Linux Command Line
- Cybersecurity Fundamentals

## Author

Ugwu Cosmas
