# Apna Bank - Command Line Banking System with Face Unlock

This is a command-line banking application written in Python. It allows users to create accounts, log in, check balances, deposit or withdraw money, and change passwords. An admin can log in using facial recognition.

## Features

- User Registration and Login
- Balance Inquiry
- Deposit and Withdrawal
- Password Change
- Admin Panel with Face Unlock (using OpenCV and LBPH)
- Data persistence using `user.csv` (Pandas)

## Requirements

- Python 3.x
- Libraries:
  - pandas
  - numpy
  - opencv-python
  - opencv-contrib-python
  - pillow
  - matplotlib

Install dependencies with:
```bash
pip install pandas numpy opencv-python opencv-contrib-python pillow matplotlib
```

## How to Use

1. Run the script:
   ```bash
   python bank2.py
   ```

2. Select from the main menu:
   - Admin Login (uses webcam for face recognition)
   - User Login
   - Create Account
   - Exit

3. Follow the prompts for transactions and actions.

## Admin Face Unlock

The face recognition system uses OpenCV's LBPH Face Recognizer. Before use, ensure that:
- You have a trained model saved as `trainer.yml`
- Your webcam is functional

Training the model is not included in this script and must be done separately.

## Data Storage

User data is stored in `user.csv` with the following columns:
- `username`
- `password` (stored as plain integer - **for demo purposes only**)
- `balance`

## Security Note

- Passwords are stored in plain text and PINs are not hashed.
- This system is intended for educational/demo purposes only.
- Do not use in production environments without significant improvements in security.

## Author

Apna Bank Command Line System - For demonstration and learning purposes.