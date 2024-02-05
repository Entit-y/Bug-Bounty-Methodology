[[Tags]] : #CLI_Tool #Recon #Directory_Discovery 

## Description :

**Dirsearch** tool is a Python language-based tool, which is command-line only. Dirsearch lights when it comes to recursive scanning, so for every directory it identifies, it will go back through and crawl the directory for some additional directories. Dirsearch tool is an advanced command-line tool designed to brute-force directories and files in web servers or web path scanners. As Dirsearch is an advanced tool, it allows hackers to perform a complex web directories discovery,  with a customized wordlist, impressive performance, speed, high accuracy, advanced correction, and modern brute-force techniques with relevant outputs.

## Usages :

- Use **dirsearch -h** to get a list of all tags
- **-o** tag is used to save the results to an output txt file(default name "dirsearch.txt")

**Simple usage:**
>dirsearch -u https://example.com -o dirsearch.txt

**Extensions (php,html,js):**
>dirsearch -e php,html,js -u https://example.com -o dirsearch.txt

**Using Wordlist:**
>dirsearch.py -e php,html,js -u https://example.com -w /usr/share/wordlists/dirb/common.txt -o dirsearch.txt

**Simple Recursive Scan:**
>dirsearch.py -e php,html,js -u https://example.com -r -o dirsearch.txt
>*for finding specific file types/extensions like php,html,js*

**Max Recursion Depth:**
>dirsearch.py -e php,html,js -u https://example.com -r -R 3 -o dirsearch.txt

**Using Threads:**
>dirsearch.py -e php,htm,js,bak,zip,tgz,txt -u https://example.com -t 30\ -o dirsearch.txt


**Prefixes:**
>dirsearch.py -e php -u https://example.com **–prefixes** .,admin,_,~ -o dirsearch.txt
>for finding specific file names like admin

**Suffixes:**
>dirsearch.py -e php -u https://example.com **–suffixes** ~,/ -o dirsearch.txt
>*for finding specific letters or symbols like ~ or /*(multiple suffixes are separated by a comma)

**Excluding Extensions:**
>dirsearch.py -e asp,aspx,htm,js -u https://geeksforgeeks.org **-X** php,jsp,jspx -o dirsearch.txt

**Filtering status codes:**
>dirsearch -u https://example.com --exclude-status 404 -o dirsearch.txt

**Scan sub-directories:**
> dirsearch.py -e php,html,js -u https://example.com –subdirs admin/,folder/,/ -o dirsearch.txt
**Using Proxy Server:**
>dirsearch.py -e php,html,js -u https://example.com –proxy 127.0.0.1:8080 -o dirsearch.txt




