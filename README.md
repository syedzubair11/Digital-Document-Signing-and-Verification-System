# Digital Document Signing & Verification System

## Overview
This project is a secure document transfer system that uses hybrid cryptography to ensure confidentiality, integrity, and authenticity of files exchanged between users. It combines symmetric encryption, asymmetric encryption, digital signatures, and a multi-user verification chain.

---

## Key Features
- Secure file encryption using AES (symmetric encryption)
- RSA-based encryption for secure AES key exchange
- SHA-256 hashing for file integrity verification
- Digital signatures for authentication
- Multi-user signature chain verification
- Certificate Authority (CA) based public key retrieval

---

## System Workflow

### 1. Encryption Phase
- File is encrypted using AES
- AES key is encrypted using recipient’s RSA public key

### 2. Integrity & Signing Phase
- SHA-256 hash is generated for the file
- Sender signs the hash using their private key

### 3. Multi-Signature Chain
- Multiple users can sequentially sign the document
- Each signature verifies the previous state of the chain

### 4. Decryption & Verification
- Recipient decrypts AES key using RSA private key
- File is decrypted using AES
- Hash and signature chain are verified using CA-provided public keys

---

## Technologies Used
- Python
- PyCryptodome
- RSA Encryption
- AES Encryption (EAX mode)
- SHA-256
- Tkinter (GUI)
- JSON-based secure packaging

---

## My Contribution
This project was developed as a group effort.

My contributions include:
- Implemented AES encryption and decryption logic
- Developed RSA-based secure key exchange system
- Implemented SHA-256 hashing and digital signature verification
- Designed and implemented multi-signature chain verification
- Integrated cryptographic workflows into a single system

---

## Security Concepts Implemented
- Hybrid Encryption (AES + RSA)
- Public Key Infrastructure (PKI concept via CA)
- Digital Signatures (PKCS#1 v1.5)
- Cryptographic Hashing (SHA-256)
- Chain of Trust verification

---

## Note
This repository is a fork of a group project. Contribution details reflect my individual work.
