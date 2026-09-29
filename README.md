# RevWho - Reverse WHOIS Domain Reconnaissance Tool

RevWho is a Python-based Open Source Intelligence (OSINT) tool designed to streamline reverse WHOIS lookups. By querying ViewDNS.info, it identifies and extracts all domain names associated with a specific company name or administrative email address.

<img width="876" height="405" alt="image" src="https://github.com/user-attachments/assets/0ac9aacd-62e2-4fe7-a513-8047ba891c91" />

---

## Features

- **Company & Email Querying:** Search using organization names (e.g., Google LLC) or registrar email addresses.
- **Automated HTML Parsing:** Extracts clean domain results directly from target web responses.
- **Robust Error Handling:** Properly handles connection timeouts, network drops, bad responses, and manual user cancellations (Ctrl+C).
- **Lightweight Footprint:** Built with standard Python modules and requests, requiring no complex setup or heavy dependencies.

---

## Prerequisites

- Python 3.6 or higher
- pip package manager

---

## Installation

1. Clone the Repository:
   git clone https://github.com/xav1ersys/revwho.git
   cd revwho

2. Install Dependencies:
   pip install requests

---

## Usage

1. Run the script from your terminal:
   python3 revwho.py

2. Enter the target organization or email address when prompted:
   Enter the company name or company email.
   Google LLC

3. The tool will parse the query and output the list of registered domains directly to the console.

---

## Technical Details

The script performs the following operations:
- URL-encodes user input to form valid HTTP requests.
- Sets a modern desktop User-Agent header to bypass basic request filtering.
- Queries the ViewDNS reverse WHOIS endpoint.
- Uses Regular Expressions (re) to parse and sanitize the HTML table output into clean domain strings.

---

## Disclaimer

This project is intended strictly for educational purposes, security research, and authorized OSINT investigations. Users are responsible for complying with all applicable local, state, and federal laws. The author assumes no liability for misuse or damage caused by this program.

Use for Good Purposes!!
---

## License

Distributed under the MIT License. See LICENSE for more information.
