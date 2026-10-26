# RSA Text Encryption and Decryption — SageMath

## Overview

This project implements an educational version of the RSA public-key cryptosystem using SageMath. It demonstrates how a text message can be converted into numerical blocks, encrypted using RSA, and recovered through decryption.

The implementation combines RSA operations with character encoding, prime-number testing, modular arithmetic, and CRT-based decryption.

## Features

- **Character encoding:** Maps supported characters to numerical codes.
- **Prime generation:** Uses the Miller–Rabin primality test to generate candidate prime numbers.
- **RSA key generation:** Computes the RSA modulus and the public and private exponents.
- **Text processing:** Converts a message into numerical character codes and groups them into blocks.
- **Encryption:** Applies modular exponentiation to encrypt the numerical blocks.
- **CRT-based decryption:** Uses the Chinese Remainder Theorem to perform RSA decryption.
- **Message reconstruction:** Converts the decrypted numerical blocks back into the original text and checks whether the message was recovered correctly.

## Technologies

- SageMath
- Jupyter Notebook interface with a SageMath kernel

## How to Run

1. Install SageMath in your Ubuntu environment through WSL.
2. Download or clone this repository.
3. Open `RSA-Text.ipynb` using a Jupyter environment configured with a SageMath kernel.
4. Execute the notebook cells in order.
5. Enter a message when prompted.
6. Observe the numerical encoding, encrypted blocks, decrypted message, and success status.

**Note:** This notebook uses SageMath-specific objects and functions, including `ZZ`, `Integer`, `gcd`, and `power_mod`. It should be executed with SageMath rather than an ordinary Python kernel.

## Documentation

The accompanying RSA report covers the mathematical foundations of RSA, key generation, encryption and decryption, a worked example, proof of correctness, security considerations, and computational complexity.

## Limitations

This project is intended for educational purposes and for studying the mathematical operations behind RSA. It is not a production-ready encryption system and should not be used to protect sensitive information.

The implementation uses a custom character encoding and a simplified RSA construction. It does not implement a complete, standardized secure text-encryption protocol.
