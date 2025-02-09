# FileThingie 2.5.7 Exploit - Arbitrary File Upload to RCE

## Description
This script exploits an arbitrary file upload vulnerability in FileThingie 2.5.7 to achieve remote code execution (RCE). It allows an authenticated user to upload and extract a PHP shell, enabling command execution on the target server.

## Features
- Logs in to the target FileThingie instance
- Creates a ZIP archive containing a simple PHP shell
- Uploads the ZIP file
- Unzips the archive, making the shell accessible

## Usage

### Prerequisites
- Python 3.x
- `requests` module installed (`pip install requests`)

### Running the exploit
```bash
python exploit.py -t <target_url> -u <username> -p <password>
```
### Disclaimer
This script is intended for educational and authorized security testing purposes only. Unauthorized use of this exploit against systems you do not own or have permission to test is illegal.

### Author
Original exploit by Maurice Fielenbach (grimlockx), modified for targeted use https://www.exploit-db.com/exploits/51436
