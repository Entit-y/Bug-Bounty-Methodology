[[Tags]] : #Recon #CLI_Tool #Subdomain_Enumeration 
## Description :

Sublist3r is a Python security tool designed to enumerate subdomains of websites using OSINT. It helps penetration testers and bug hunters collect and gather subdomains for the domain they are targeting over the network. Sublist3r enumerates subdomains using many search engines such as Google, Yahoo, Bing, Baidu, and Ask. Sublist3r also enumerates subdomains using Netcraft, Virustotal, ThreatCrowd, [[DNS_dumpster]], and ReverseDNS.

## Usage:

- Use **sublist3r -h** to get a list of all tags
- -o tag is used to save the results to an output txt file(default name "sublister.txt")

**Example:** 
To list the subdomains of a domain enter the following command in Linux and replace “kali.org” with the website you want to list the subdomains of.
```bash
sublist3r -v -d example.com -t 5 -o ~/Desktop/sublister.txt
```

Where -d stands for domain listing and -v will verbose the output and tell from where it is getting the results. The fetch results will be saved in subresult.txt file in the desktop directory and the number of threads will be 5.