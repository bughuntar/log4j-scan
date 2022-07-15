# log4j-scan
A fully automated, accurate, and extensive scanner for finding log4j RCE CVE-2021-44228


**Installation:**
```javascript
sudo git clone https://github.com/fullhunt/log4j-scan.git && cd log4j-scan && sudo chmod +x * && sudo pip3 install -r requirements.txt
```

**Scan:**
Scan a Single URL using all Request Methods: GET, POST (url-encoded form), POST (JSON body)
```javascript
python3 log4j-scan.py -u https://log4j.lab.secbot.local --run-all-tests
```
Discover WAF bypasses against the environment.
```javascript
python3 log4j-scan.py -u https://log4j.lab.secbot.local --waf-bypass
```
Scan a list of URLs
```javascript
python3 log4j-scan.py -l urls.txt
```
