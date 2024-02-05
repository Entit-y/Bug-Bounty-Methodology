[[Tags]] : #Testing #Bug 

## Description :

Cross-site scripting (also known as XSS) is a bug that allows an attacker to compromise the interactions that users have with a vulnerable application. It allows an attacker to circumvent the same origin policy, which is designed to segregate different websites from each other. Cross-site scripting vulnerabilities normally allow an attacker to masquerade as a victim user, to carry out any actions that the user is able to perform, and to access any of the user's data. If the victim user has privileged access within the application, then the attacker might be able to gain full control over all of the application's functionality and data.
for more info on XSS check out :[Port Swigger XSS](https://portswigger.net/web-security/cross-site-scripting)

![[cross-site-scripting.svg]]

## Testing :
#### Reflected :
	- Manually submit unique input in every input field you can find on the target and Identify every location on the target where this input was reflected in the http response
	- Make sure to submit every single key on the keyboard at every input field you can find. this is to determine which keys are being black listed by the waf.
> you can use the [[XSS Vibes]] tool to check for black listed and allowed inputs on an endpoint


## Proof Of Concept's :

1. [[$6,000 Bounty for XSS _ Bug Bounty 2023]]

![[$6,000 Bounty for XSS _ Bug Bounty 2023.mp4]]

2. [[Bug Bounty POC - Blind XSS]] :

![[Bug Bounty POC - Blind XSS.mp4]]

3. [[Cookie Based XSS _ Bug Bounty Poc]] :

![[Cookie Based XSS _ Bug Bounty Poc 1.mp4]]

4. [[Cross Site Scripting Via Cookies Bug Bounty Poc:]]

![[Cross Site Scripting Via Cookies Bug Bounty Poc.mp4]]

5. [[Cross Site Scripting Vulnerability Bug Bounty Poc]]:

![[Cross Site Scripting Vulnerability Bug Bounty Poc.mp4]]

6. [[Poc of xss in gitlab worth $13950 Hackerone]]:

![[Poc of xss in gitlab worth $13950🤑 _ Hackerone.mp4]]

7. [[POC_XSS_CSRF]]:

![[POC_XSS_CSRF.mp4]]

8. [[Reflected xss bug bounty poc]]:

![[Reflected xss bug bounty poc.mp4]]

9. [[Simple host header injection vulnerability poc _ bug bounty]]:

![[Simple host header injection vulnerability poc _ bug bounty _.mp4]]

10. [[Cross Site Scripting Reflected XSS Vulnerability]]
![[Cross Site Scripting Reflected XSS Vulnerability.mp4]]

11. $800 Advanced Stored Cross Site Scripting Filter Bypass to Account Takeover
![[$800 Advanced Stored Cross Site Scripting Filter Bypass to Account Takeover _ Bug Bounty PoC 2024.mp4]]
13.Cracking Websites with Cross site scripting
![[Cracking Websites with Cross Site Scripting.mp4]]

14.Cookie based XSS Asana bug bounty
![[Cookie Based XSS _ Asana _ Bug Bounty POC.mp4]]

15. XSS via file name ![[XSS via  File Name.mp4]]
16. XSS via file upload ![[File upload to XSS _  Bug Bounty Hunting - XSS Through File Uploading  _ Bug Bounty _ POC.mp4]]
17. XSS on Lenovo via file upload ![[Lenovo XSS via Unrestricted File Upload PoC.mp4]]
18. XSS POC ![[Xss Poc __ xss __ Cross Site Scirpting.mp4]]
19. XSS via cookie in Bluehost.com ![[XSS via Cookie in Bluehost.com _ POC video _  BugCrowd _  UnFixed.mp4]]
20. Cookie based XSS on netmeds.com ![[Cookie Based XSS _ Bug Bounty Poc 1.mp4]]
21. Swagger API to XSS ![[Swagger API to XSS on IBM _ Bug Bounty POC 1.mp4]]



































