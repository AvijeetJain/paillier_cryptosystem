# Paillier Cryptosystem

This repository provides an implementation of the **Paillier Cryptosystem**, a probabilistic public-key cryptosystem with additive homomorphic properties. This implementation allows for encrypting, decrypting, and performing computations directly on encrypted data.

---

## Features

- **Public-Key Encryption**: Securely encrypt and decrypt messages using a public-private key pair.
- **Additive Homomorphism**: Perform addition of plaintexts on encrypted data without decrypting.
- **Flexible and Modular**: Easily integrate into cryptographic workflows.

---

## Prerequisites

Ensure you have the following installed:
- Python 3.8 or later

---

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Navigate to the directory:
   ```bash
   cd pallier-crypto-system
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. **Generate Key Pair**:
   ```python
   from pallier import KeyGenerator

   keygen = KeyGenerator()
   public_key, private_key = keygen.generate_keys()
   ```

2. **Encryption**:
   ```python
   ciphertext = public_key.encrypt(plaintext)
   ```

3. **Decryption**:
   ```python
   decrypted_message = private_key.decrypt(ciphertext)
   ```

4. **Homomorphic Addition**:
   ```python
   result = public_key.add(ciphertext1, ciphertext2)
   ```

---

## Files

- **`pallier.ipynb`**: Jupyter notebook containing the implementation and examples.
- **`README.md`**: Documentation for the project.
- **`.gitignore`**: Excludes unnecessary files from version control.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to suggest improvements or report bugs.

---

## Acknowledgments

The implementation is based on the paper by Pascal Paillier (1999).
