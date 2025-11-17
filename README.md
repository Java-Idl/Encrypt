# Encrypt

## AES File Encryption/Decryption

A simple, secure web app for encrypting and decrypting files right in your browser using AES-256-GCM encryption with PBKDF2 key derivation.

***

## Features

- **Encrypt files** with a password (8-32 characters).
- **Decrypt files** encrypted by the app using the correct password.
- Uses **AES-256-GCM** for top-level security.
- PBKDF2 with 310,000 iterations for strong password-based key derivation (OWASP recommended for 2025).
- Clean, modern UI with real-time password strength feedback.
- Shows file size info before and after encryption/decryption.
- Progress bar during encrypt/decrypt operations.
- Download encrypted or decrypted files easily.

***

## How to Use

1. Open the page in a modern browser that supports the Web Crypto API.
2. Switch between **Encrypt** and **Decrypt** tabs as needed.
3. For encryption:
   - Select the file you want to encrypt.
   - Enter a strong password (minimum 8 characters, max 32).
   - Click **Encrypt File**.
   - Wait for the process to finish, then download the encrypted file.
4. For decryption:
   - Select the encrypted file.
   - Enter the password used for encryption.
   - Click **Decrypt File**.
   - Download the decrypted original file.

***

## Notes

- Encryption adds a salt and nonce to the output to ensure security and uniqueness.
- Passwords are never stored or sent anywhere; all work is done locally in your browser.
- Make sure to remember your password; losing it means you can't decrypt your files.
- Supports files of any type.
- The UI is responsive and works well on mobile and desktop.

***

## Security

- **AES-256-GCM** encryption.
- Password key derived using **PBKDF2** with 310,000 iterations and SHA-256.
- Salt and nonce are generated randomly for each encryption to prevent reuse attacks.
- Trusted Web Crypto API ensures strong cryptographic operations client-side.

***

## Tech Stack

- Vanilla HTML, CSS, and JavaScript.
- Web Crypto API for cryptography.
- No server/backend — pure client-side app.

***

## License

Feel free to use, modify, and share. No warranties. Use at your own risk.

***

Enjoy your secure file encryption! 🔐
