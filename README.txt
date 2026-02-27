# 🛡️ My Vault: Secure Terminal

**A local-first, hardware-bound security terminal designed to keep your digital identity under a physical lock and key.**

Developed as a Computer Engineering student project, **My Vault** explores the intersection of Python-based cryptography and hardware-linked authentication. It uses AES-256 military-grade encryption to secure your data, but with a twist: it requires both a Master Password *and* a physical USB "Bone-Key" to decrypt the database. 

Zero cloud, zero telemetry. Your data stays with you.

---

## 🚀 Key Features
* **Physical Layer Security:** The database is mathematically locked to a specific file on your USB drive. No USB, no access.
* **Military-Grade Core:** Powered by AES-256 (Advanced Encryption Standard).
* **Cyber-Immersion UI:** A custom-built, low-latency terminal interface with immersive dark-mode aesthetics.
* **Brute-Force Protection:** Integrated lockout system that triggers after failed login attempts.

---

## 🔑 Initial Setup: Forging Your Hardware Key
To use My Vault, you must set up a physical security key first. **Do not skip this step!**

1. Insert a USB Drive into your computer.
2. Create a new, plain text file on the drive and name it `vault_key.txt`.
3. Open the file and paste exactly this text inside (no extra spaces): 
   `DARYAN_OMEGA_PROTOCOL_2026`
4. Save the file. **Keep this USB safe!** If you lose it, your vault remains permanently locked.

---

## 🛠️ How to Use the Terminal
1. **Launch:** Run the `vault_app.exe` file.
2. **Master Password:** Enter the default system password: `daryan`
3. **Hardware Handshake:** Click the button to insert/load your hardware key, and navigate to the `vault_key.txt` file on your USB drive.
4. **Authenticate:** Click to decrypt. If the password and the USB key match the encryption matrix, you will be granted access to the secure subnet.
5. **Manage Data:** From the dashboard, you can add new nodes (passwords), generate secure keys, and view your encrypted activity logs.

---

## 🏗️ Technical Architecture
* **Language:** Python 3.2
* **GUI Framework:** Tkinter (Customized for Immersive Dark Mode)
* **Security:** `cryptography.fernet` (Symmetric Encryption)
* **Packaging:** PyInstaller (Standalone Executable bundling data and assets)

---

## 📜 About the Developer
Developed by **Daryan Amanj**, Computer Engineering student. This project was built to demonstrate secure system design, symmetric cryptography, file I/O operations, and custom GUI engineering.