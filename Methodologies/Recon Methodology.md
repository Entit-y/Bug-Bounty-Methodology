Start out your recon with a [[Webcopilot]] and [[Nmap-Automator]] scan
And utilize [[HackerGPT]]

Subdomain enumeration:

Use the crt.sh website

[[subfinder]] 
> subfinder -d example.com(there's some extra flags you should learn about)

[[sublist3r]]
>sublist3r -v -d example.com -t 5 -e bing -o ~/Desktop/subresult.txt

[[Dirsearch]] 
> dirsearch -u example.com (theres some extra flags you should learn about)

Try out Project Discovery's tool called "chaos"
Try out the DNSDumpster website

Js enumeration:
Burpsuite
subjs
Secretfinder.git | Linkfinder.git

Shodan Enumeration > "ssl:"Target.com" " | ssl.cert.subject.CN:"Target.com" 200 | https://www.shodan.io/search?query=http.favicon.hash%3ATARGETSHASh

Vulnerability enumeration:

Nuclei > nuclei -c 150 -l "ips.txt" -severity unknown,low,medium,high,critical -etags "intrusive" -o "VulnsIP.txt"

socialhunter(used for broken link hijacking *do research on that*)

*Note: get the "Trufflehog" browser extension, it's used to find secrets in a webpage

Some keywords to search for when testing subdomains: admin, dev, secure, remote(could lead to vpn)

USE HACKTRICKS AND RSON METHODOLOGY FOR TESTING

Use some _Some Google dorks_ [^1]

For some word lists try out: https://github.com/SupremeERG/Bug-Bounty-Wordlists/tree/main






































## References: 
[^1]: [[Google Hacking Dorks.pdf]]



