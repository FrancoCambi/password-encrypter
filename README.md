# Simple Password Encryptor/Decryptor (C)

This is a basic password encryption and decryption program written in C. It uses XOR with a static key to encrypt and decrypt strings, displaying the encrypted result in hexadecimal format.

This proyect was made just for fun and some learning :)

---

## Features

- Encrypt any text string using a static XOR key.
- Decrypt a hexadecimal string back to its original text.
- Simple terminal-based menu.
- Works on both Linux and Windows.

---

## How It Works

- **Encryption**: The input string is XOR'd with a predefined key and converted to a hexadecimal representation.
- **Decryption**: The input hexadecimal string is parsed into bytes, XOR'd with the key, and reconstructed into the original text.

---

## Usage

1. **Compile the program**:

   ```bash
   gcc -o encryptor main.c
   ```

2. **Run the program**:

   ```bash
   ./encryptor
   ```

3. **Choose an option**:
   - `1` to encrypt a string
   - `2` to decrypt a hexadecimal string
   - `3` to exit

---

## Example

```
Encrypt or decrypt? (1 | 2 | 3 to exit) 1

String: hello
Encrypted to: 1b111e0501

Encrypt or decrypt? (1 | 2 | 3 to exit) 2

Hexadecimal: 1b111e0501
Decrypted to: hello
```

---

## Notes

- The encryption key is hardcoded as `"stringkey"`.
- Encryption is **not secure** for real password storage or sensitive data.
- This tool is for educational or demonstration purposes only.

---

## License

This project is released under the MIT License.

