# 🔐 Password Breach Checker

This project is a simple command-line tool that checks whether a password has been exposed in known data breaches. It uses the **HaveIBeenPwned API** with **SHA-1 hashing** and the **k-anonymity model** to ensure privacy.

---

## 🧠 How It Works

1. Takes a password input from the user.
2. Hashes the password using SHA-1.
3. Sends the first 5 characters of the hash to the API.
4. Receives a list of matching suffixes and compares to the full hash.
5. Displays the number of breaches the password appeared in.

All while preserving full password anonymity.

---

## 🛠️ Technologies Used

- Python 3
- `hashlib`
- `requests`
- HaveIBeenPwned API (public and free)

---

## 🚀 How to Run

```bash
$ python password_breach_checker.py
Enter a password to check: password123
⚠️ Password found in 864904 breaches! Choose a stronger one.

💡 Use strong, unique passwords. Avoid anything commonly used or leaked.

