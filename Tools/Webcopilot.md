[[Tags]] : #Recon #CLI_Tool #Automated

## Description : 

**WebCopilot** is an automation tool designed to enumerate subdomains of the target and detect bugs using different open-source tools.

The script first enumerate all the subdomains of the given target domain using assetfinder, sublister, subfinder, amass, findomain, hackertarget, riddler and crt then do active subdomain enumeration using gobuster from SecLists wordlist then filters out all the live subdomains using dnsx then it extract titles of the subdomains using httpx & scans for subdomain takeover using subjack. Then it uses gauplus & waybackurls to crawl all the endpoints of the given subdomains then it use gf patterns to filters out xss, lfi, ssrf, sqli, open redirect & rce parameters from that given subdomains, and then it scans for vulnerabilities on the subdomains using different open-source tools (like kxss, dalfox, openredirex, nuclei, etc). Then it'll print out the result of the scan and save all the output in a specified directory.

## Usage : 

- Use **sudo webcopilot -h** to get a list of all tags
- `-o` tag is used to save the results to an output txt file(default name "copilot_scan.txt")

**simple usage:**
```bash
sudo webcopilot -d example.com -o copilot_scan.txt
```

The `-s` command can be used for only subdomain enumerations:
```bash
sudo webcopilot -d example.com -o copilot_scan.txt -s
```

The `-t` command can be used to add thrads to your scan for faster result:
```bash
sudo webcopilot -d example.com -o copilot_scan.txt -t 10
```

The `-b` command can be used for blind xss (OOB), you can get your server from [xsshunter](https://xsshunter.com/) or [interact](https://interact.projectdiscovery.io/):
```bash
sudo webcopilot -d example.com -o copilot_scan.txt -t 10 -b testServer.xss
```

The `-x` command can be used to exclude out of scope domains:
```bash
echo out.example.com > excludeDomain.txt
sudo webcopilot -d example.com -o copilot_scan.txt -t 10 -x excludeDomain.txt -b testServer.xss
```

