# 🚀 Server Interaction Automation Tool

This project is a Python-based utility designed to automate the discovery and handling of low-population servers
via API scraping, image-based screen recognition, and scripted key events. It integrates OCR (Optical Character
Recognition), real-time input simulation, and persistent logging to streamline repetitive tasks that would 
otherwise be performed manually.

## Features

- ✅ Server list acquisition and filtering via API
- 🔍 OCR-based UI element detection using `pytesseract`
- 🎯 Automatic macro execution via `keyboard` and `mouse` inputs
- 📊 Persistent Excel logging of server usage and autoskip history for further analysis
- 🧠 Intelligent management of servers reuse avoidance based on external rules of the site
- 🧼 Automatic cleanup of expired server entries
- 📸 Screenshot logging of OCR state when detection fails mostly for increasing accuracy

## Technologies Used

- `Python 3`
- `requests` – for API requests
- `pytesseract` – OCR integration (requires Tesseract OCR)
- `Pillow`, `OpenCV` – for image processing and enhancement
- `keyboard`, `mouse`, `pyperclip` – for simulating user input
- `openpyxl` – for Excel file manipulation
- `json`, `datetime`, `threading` – for data persistence and concurrency

## Requirements

- Tesseract OCR installed and accessible
- Python packages (install via `pip install -r requirements.txt`):


## How to use

 Launch the `get_empty_servers` script in a Python 3 environment.

The tool will:
- Fetch a list of servers from the API

- Filter out populated or recently used servers

- Copy connection strings to clipboard

- Simulate interaction and detect "Warmup" status via OCR

- Log activity and skip servers as needed


The tool is intended for automating repetitive connection and status-checking tasks.
Server cooldown is enforced to avoid reusing recently attempted entries.
Logs and screenshots are stored in local directories for later inspection.

## ⚠️ Important Notice

This tool was created as a favor for a friend and primarily for **educational purposes**.  
I do **not** encourage or endorse its use. If you choose to use this tool, you do so at your **own risk** 
and accept full responsibility for any consequences, including a **high probability of being banned**.

**Use responsibly.**