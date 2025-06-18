File Change Monitor (Hash-Based) – PyQt5 GUI

This Python application lets you monitor any changes in files within a folder using SHA-256 hashing. Whether you're detecting tampering, tracking updates, or just keeping an eye on important files — this tool makes it easy with a simple GUI.

Preview
<img width="1072" alt="Screenshot 2025-06-18 at 11 24 30 PM" src="https://github.com/user-attachments/assets/756d3440-7e22-4da7-8345-cb74084f37ca" />



Features:
- Select any folder via GUI
- Automatically detects New, Modified, or Deleted files
- Displays results in a clear table
- Saves previous hash states in a JSON file
- Lightweight, fast, and user-friendly

Requirements :
Python 3.7 or newer

PyQt5 (GUI library)

Install dependencies:

bash
Copy
Edit
pip install PyQt5

How to Run:
bash
Copy
Edit
python file_monitor.py
Replace file_monitor.py with your script filename if it's different.

How It Works:
Click "Select Folder" to pick a directory.

Click "Scan & Compare" to:

Generate SHA-256 hashes for all files

Compare current hashes with stored ones

Detect and show NEW, MODIFIED, and DELETED files

Results are shown in a table.

Hashes are saved in file_hashes.json for future runs.

About file_hashes.json
Automatically created on first scan.

Stores a snapshot of file paths and their corresponding hashes.

Keeps history for comparison during future scans.

Delete this file to reset all history.

Notes:
Works recursively — includes subfolders too.

Avoid using this on system folders or very large directories.

