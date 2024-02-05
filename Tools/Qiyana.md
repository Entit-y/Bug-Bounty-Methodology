[[Tags]] : #Recon #CLI_Tool  #Directory_Discovery #Subdomain_Enumeration #Parameter_Fuzzing

## Description :

Qiyana is a python tool for fuzzing directories, parameters, etc.. Created with Python3.
You can find it in your Recon/Parameter_Fuzzing Directory

## Usage :

- Use **python3 Qiyana.py -h** to get a list of all tags
- **-o** tag is used to save the results to an output txt file(default name "Qiyana.txt")

**simple usage:**
```bash
qiyana.py -u https://example.com -w wordlist-path -o Qiyana.txt
```

**follow redirects:**
```bash
Qiyana.py -u https://example.com -f -w wordlist-path -o Qiyana.txt
```

**parameter fuzzing:**
```bash
python3 Qiyana.py -u https://example.com -P -w wordlist-path -o Qiyana.txt
```


**subdomain enumeration**:
```bash
python3 Qiyana.py -u https://example.com -S -w wordlist-path -o Qiyana.txt
```

