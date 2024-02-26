```markdown
# Cybersecurity Toolkit

## Reconnaissance

### DNS Enumeration:
- `nslookup (website)`
- `whois (website)`

### Information Gathering:
- `theHarvester -d (domain) -b`

### Port Scanning:
- `nmap -A -F -T1 192.168.8.1`

## Web Application Testing

### Directory Bruteforcing:
- `ffuf -w /usr/share/wordlists/dirb/common.txt -u http://tenet.htb/FUZZ -fc 403 -p 1`

### WordPress Scanning:
- `wpscan --url (domain) -e ap --plugins-detection aggressive`

## Tools Installation

### SecLists Installation:
```bash
git clone https://github.com/danielmiessler/SecLists.git
cd SecLists/Discovery/
```

### Shodan Initialization:
- `shodan init (api key)`

### Go Programming Language Installation:
- `sudo apt install golang`

## Passive Reconnaissance

### Amass Passive Enumeration:
- `amass enum -passive -d (domain)`

### Subdomain Enumeration:
- `sublist3r -d (domain)`
- `amass enum -d (domain)`

## Active Reconnaissance

### Host Discovery:
- `host ( .com)`
- `ping .com`
- `shodan host ( ip)`

### Shodan Scanning:
- `shodan scan submit (ip)`

### Zone Transfer:
- `dig axfr @(ip) friendzone.red`
- `dig axfr @(ip) friendzone.red > (file name)`

## Miscellaneous

### File Manipulation:
- `gunzip wordpressfile.json.gz`
- `cat wordpressfile.json | grep friendzone | grep IN | awk '{print $1}'`

### Text Editing:
- `sudo apt install gedit`
- `gedit nom.txt`

### Miscellaneous Tools:
- `ls`
- `clear`
```
