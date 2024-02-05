[[Tags]] #Testing #Bug 

## Description:

Server-side request forgery(SSRF) is a bug that allows an attacker to send specially crafted requests to a server that causes the server to make requests to an arbitrary URL on behalf of the attacker.
This can allow the attacker to steal sensitive information or perform actions on behalf of the attacker


## Testing:
	- Take note of all requests with parameters that contain ip-addresses whether internal ip's(192.168.x.x) or external ip's.
	- Also take note of whether an application uses user input to generate a url which is then used to make a request


## Proof Of Concept's :

1. $1,913 Unauthenticated SSRF Leading To Interal Port Scanning _ Bug Bounty POC 2023 _ P3 Severity ![[$1,913 Unauthenticated SSRF Leading To Interal Port Scanning _ Bug Bounty POC 2023 _ P3 Severity.mp4]]
2. Blind SSRF_ User Ip discloser via image url ![[Blind SSRF_ User Ip discloser via image url _ VDP _ Bug Bounty Poc _ $$.mp4]]
3. Escalating HTMLI To SSRF POC ![[Escalating HTMLI To SSRF POC.mp4]]
4. External service interaction poc ![[External service interaction poc.mp4]]
5. SSRF in Dukaan Bug Bounty Program _ Bug Bounty POC 2023 ![[SSRF in Dukaan Bug Bounty Program _ Bug Bounty POC 2023.mp4]]
6. SSRF Vulnerability (Filters Bypass) - PoC ![[SSRF Vulnerability (Filters Bypass) - PoC.mp4]]
7. ssrf vulnerability exploit __ ssrf __ bug bounty poc 2023 __ site hack __ ssrf in cloud servis ![[ssrf vulnerability exploit __ ssrf __ bug bounty poc 2023 __ site hack __ ssrf in cloud servis.mp4]]



















































