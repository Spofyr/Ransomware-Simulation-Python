# Ransomware-Simulation-Python
Academic cybersecurity project demonstrating AES-128 encryption and Trojan-horse delivery. (EST Guelmim - RIS)
# Ransomware & Trojan Simulation

**Author:** Aymane El Allali  
**Program:** Computer Systems Networking & Security (RIS)  
**Institution:** EST Guelmim

## Project Overview
This project is a Proof-of-Concept (PoC) developed for academic purposes. It simulates a ransomware attack chain, focusing on symmetric encryption and payload delivery via a Trojanized executable.

## Technical Details
- **Encryption:** AES-128 Symmetric encryption using the `cryptography.fernet` library.
- **Payload Delivery:** The script is compiled into a `.exe` using **PyInstaller**, disguised with a PDF icon to simulate social engineering.
- **Environment:** Tested within an isolated **Windows Sandbox**.


## How to Run (Educational Use Only)
1. **Setup Environment:**
   `pip install cryptography pyinstaller`
2. **Compile to Executable:**
   `python -m PyInstaller --onefile --noconsole --icon=your_icon.ico malware.py`
3. **Usage:**
   - Run `.\malware.exe encrypt` to lock files in the target directory.
   - Run `.\malware.exe decrypt` to restore them using the generated key.

## Disclaimer
This repository is for educational and authorized security testing only. Malicious use of this code is strictly prohibited.
