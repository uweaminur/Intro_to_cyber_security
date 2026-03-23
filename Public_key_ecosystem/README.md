# Public Key (RSA) Cryptography Simulator

A lightweight, client-side web application that visualizes the flow of Asymmetric Cryptography over an untrusted network. 

This simulator uses the browser's native **Web Crypto API** to generate real 2048-bit RSA keys, proving that mathematical encryption can secure data even when the transmission medium (the internet) is compromised.

## 🔒 Core Concepts Demonstrated

1. **Key Generation:** Bob generates a mathematically linked key pair. He shares the *Public Key* openly but tightly guards the *Private Key*.
2. **Encryption (Locking):** Alice uses Bob's openly available Public Key to scramble her plaintext message into ciphertext.
3. **The Interception (Eve):** The ciphertext travels across the network. A hacker (Eve) intercepts it. Even if Eve has Bob's Public Key, she cannot decrypt the message. Public keys lock; they do not unlock.
4. **Decryption (Unlocking):** Bob receives the ciphertext and applies his Private Key—the only mathematical key in existence capable of reversing the encryption—revealing the original message.

## 🚀 How to Use

Because this project runs entirely in the browser, there are no dependencies to install.

1. Clone this repository or download `index.html`.
2. Open `index.html` in any modern web browser.
3. Follow the numbered steps on the dashboard: Generate Keys -> Encrypt & Send -> Intercept -> Decrypt.

## 🛠️ Technology Stack

* **HTML5 / CSS3:** Uses CSS Grid for a clean, responsive dashboard layout.
* **Vanilla JavaScript:** Handles the simulated network flow and state changes.
* **Web Crypto API (`crypto.subtle`):** Implements real `RSA-OAEP` key generation, encryption, and decryption algorithms.

## 📝 License
This project is open-source and available for educational and personal portfolio use.
