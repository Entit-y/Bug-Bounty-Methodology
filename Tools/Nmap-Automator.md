[[Tags]] : #Recon #CLI_Tool #Port_Scanning 

## Description : 

A script used to automate recon and enumeration, it contains several other tools such as nikto, ssl scan, etc..

## Usage :

- Use **nmapauto -h** to get a list of all tags
- **-o** tag is used to save the results to an output txt file(default name "nmapAuto.txt")

Scan Types:
```
Network : Shows all live hosts in the host's network (~15 seconds)
	Port    : Shows all open ports (~15 seconds)
	Script  : Runs a script scan on found ports (~5 minutes)
	Full    : Runs a full range port scan, then runs a thorough scan on new ports(~5-10 minutes)
	UDP     : Runs a UDP scan "requires sudo" (~5 minutes)
	Vulns   : Runs CVE scan and nmap Vulns scan on all found ports (~5-15 minutes)
	Recon   : Suggests recon commands, then prompts to automatically run them
	All     : Runs all the scans (~20-30 minutes)
```

**simple usage:**
```bash
nmapauto -H example.com -t Basic -o /home/entity/Desktop/
```

**all scans:**
```bash
nmapauto -H example.com -t All -o /home/entity/Desktop/
```

