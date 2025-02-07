# 🔐 Rabin Encryption & Digital Signature

This project implements **Rabin encryption** and **digital signatures** using **large prime numbers, modular arithmetic, and the Chinese Remainder Theorem (CRT)**. It was developed as a **university assignment** for studying cryptographic algorithms.

## 📜 Features
- **Key Generation**: Generates large prime numbers `p` and `q`, ensuring they are congruent to `3 mod 4`.
- **Encryption**: Uses Rabin's quadratic residue method for secure encryption.
- **Decryption**: Recovers four possible plaintexts using **CRT**.
- **Digital Signatures**: Implements a signing and verification mechanism.
- **Comprehensive Documentation**: Includes a **PDF report** explaining the algorithm and implementation.

## 🛠️ Technologies
- **Language**: Python (SageMath)
- **Concepts**: Number theory, modular arithmetic, prime number generation

## 📄 Documentation
A **detailed PDF report** is included, explaining:
- The Rabin cryptosystem
- Mathematical foundations
- Implementation details
- Code structure

## 🚀 Usage
```python
p, q, n = generate_key()
message = 7
ciphertext = encrypt(message, n)
m1, m2, m3, m4 = decrypt(ciphertext, p, q)
signature = sign(message, p, q)
is_valid = verify(signature, message, n)
```

## 📌 University Project
This project was completed as part of a Discrete Models course assignment at ELTE.
