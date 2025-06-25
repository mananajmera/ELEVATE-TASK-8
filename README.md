# ELEVATE-TASK-8

# 🔐 Password Strength Analyzer & Custom Wordlist Generator

A Python-based tool to analyze password strength using `zxcvbn` and generate custom wordlists from user inputs for penetration testing or cybersecurity research.

---

## 🚀 Features

- **Password Strength Analysis** using Dropbox’s `zxcvbn`
- **Custom Wordlist Generator** based on user-provided information (name, DOB, pet, etc.)
- Includes:
  - Leetspeak conversion
  - Reversed strings
  - Appended years or common patterns
- Exports wordlist in `.txt` format for cracking tools (Hydra, John, Hashcat, etc.)
- CLI-based interface (GUI available via `tkinter` as optional)

---

## 📁 Project Structure

password_tool/
├── main.py # Main CLI tool
├── password_analyzer.py # Password strength analyzer
├── wordlist_generator.py # Wordlist generator logic
├── gui_interface.py # Optional GUI version
├── wordlist.txt # Output wordlist
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🛠️ Installation

### Requirements

- Python 3.x
- pip

### Install Dependencies

pip3 install zxcvbn nltk
Optional (for GUI):
sudo apt install python3-tk


⚙️ Usage
CLI Usage
python3 main.py -p "<password>" -i <name> <dob> <pet> -o output.txt
Example:
python3 main.py -p "Manan@123" -i Manan Jain 2002 Dog -o mylist.txt
GUI Usage (Optional)
python3 gui_interface.py
📦 Create Executable (Optional)
To make a standalone .exe or binary:


pip3 install pyinstaller
pyinstaller --onefile main.py
Executable will be in the dist/ folder.

📤 Sample Output
Password Analysis Result:


Score: 3 / 4
Estimated Crack Time: 3 hours (offline slow hashing)
Suggestions:
- Avoid common names or dates
- Add more unique characters or symbols
Wordlist Generated (mylist.txt):

python-repl

manan
manan2002
2002manan
jain
jain123
d0g
...

⚠️ Disclaimer
This tool is intended for educational and ethical penetration testing only.
Do not use on unauthorized systems. Misuse may be illegal.

🙌 Contribution
Pull requests are welcome. Fork the repo and improve the tool!

📜 License
This project is licensed under the MIT License.

yaml
Copy
Edit

---
