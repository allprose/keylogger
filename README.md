Keylogger
This Keylogger captures and logs all keystrokes typed on the system. The logs are saved to a local file and encrypted for security. The tool is cross-platform, working on Windows, macOS, and Linux, and can be set to run automatically at system startup.

Key Features:
Keystroke Logging: Captures all keyboard inputs and logs them to a file.
Encrypted Logs: Automatically encrypts the log file when the program is stopped, ensuring the logs are protected.
Persistent Logging: Option to start automatically at system boot.
Cross-Platform: Works on Windows, macOS, and Linux.
Automatic Installation of Dependencies: The script installs required dependencies (such as cryptography) automatically without requiring a restart.
Requirements:
Python 3.x
pynput and cryptography libraries (automatically installed by the script)
How to Run:
Download the script and save it as keylogger.py.

Run the script:

Linux/macOS:
sudo python3 keylogger.py

Windows:
python keylogger.py

The script will automatically install dependencies (if missing) and start logging keystrokes.

Stop the script using Ctrl+C to terminate it. The logs will be encrypted and saved.

Startup Configuration:
Windows: The script creates a batch file in the Startup folder to ensure the keylogger runs when the system starts.
Linux/macOS: The script modifies the .bash_profile to start the keylogger on system boot.
The keylogger will begin logging all keyboard inputs to the file ~/.keylogger_log.txt.
Upon stopping, the log file will be encrypted and saved securely.

Important Notes:
Educational Use Only: This tool is intended for security testing and educational purposes only. Do not use this tool without proper permissions from the system owner.
Admin Privileges: Running the script with root or administrator privileges is recommended for full functionality.

Log Encryption:
The log file is encrypted using the AES encryption algorithm. The key is automatically generated and saved in the keylogger.key file.
To decrypt the log file, use the same key and the decryption process provided in the script.

Author: EY
