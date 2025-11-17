# Encrypt

## AES File Encryption/Decryption Thingy

Hey, I made this web tool for encrypting and decrypting files right in your browser. It uses AES-256-GCM encryption which is like super secure? And PBKDF2 stuff to make keys from passwords. Basically, no server involved - everything happens on your computer.

***

## What It Does

- **Encrypt files** with a password (needs 8-32 characters)
- **Decrypt files** if you have the right password
- Uses **AES-256-GCM** - apparently the military uses this?
- PBKDF2 with like 310,000 iterations (this security group OWASP says it's good for 2025)
- Clean-ish UI that shows if your password sucks
- Shows file sizes before/after so you see the overhead
- Progress bar so you know it's not frozen
- Download buttons work normally

***

## How to Use It (Super Easy)

1. Open it in Chrome/Firefox/Edge (needs Web Crypto support)
2. Pick **Encrypt** or **Decrypt** tab
3. To encrypt:
   - Choose your file
   - Type a decent password (8 chars min)
   - Hit **Encrypt File**
   - Wait for the bar to finish → download encrypted file
4. To decrypt:
   - Pick the encrypted file
   - Type the EXACT password (seriously don't forget it)
   - Click **Decrypt File**
   - Download your original file

***

## Important Stuff

- Adds random "salt" and "nonce" to encrypted files (makes them extra secure)
- Passwords NEVER leave your browser (pinky swear)
- **DO NOT FORGET YOUR PASSWORD** or your files are gone forever
- Works with ANY file type (tested with memes and PDFs)
- Mobile-friendly-ish (looks okay on phones)

***

## Security Deets

- **AES-256-GCM** encryption (top tier apparently)
- Keys made with **PBKDF2** (310k iterations + SHA-256)
- New salt/nonce every time so hackers can't reuse stuff
- Uses the browser's built-in crypto thing so it's legit

***

## Tech Stuff

- Basic HTML/CSS/JavaScript (no fancy frameworks)
- Web Crypto API does all the heavy lifting
- Zero backend - your files never hit a server

***

## License

Do whatever with it, but no guarantees. If you lose your thesis, not my fault ¯\_(ツ)_/¯

***

Hope it helps keep your stuff safe! 🔐 (emoji necessary)

Enjoy your secure file encryption! 🔐
