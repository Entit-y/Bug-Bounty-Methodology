[[Tags]] : #Testing #Bug #Authenticated_Testing 

## Description : 
Insecure direct object references (IDOR) are a type of [access control](https://portswigger.net/web-security/access-control) vulnerability that arises when an application uses user-supplied input to access objects directly. The term IDOR was popularized by its appearance in the OWASP 2007 Top Ten. However, it is just one example of many access control implementation mistakes that can lead to [access controls](https://portswigger.net/web-security/access-control) being circumvented. IDOR vulnerabilities are most commonly associated with horizontal privilege escalation, but they can also arise in relation to vertical privilege escalation.

## Testing :
	- Identify any content on the application that retrieves any sensitive data ("My account" or "Profile" pages are usually good endpoints for this) and intercept the request with Burp, send to repeater and analyze the request. Most applications send ID's through their cookies so you can start by analysing it. Cookies contain multiple identifiers to be used by the application or 3rd party services. To find the relevant Identifier that is used by the application to retrieve sensitive data, you can start by removing an Identifier, sending the request and checking the response to if any relevant changes was made. The response code is most likely to change if a relevant cookie is removed 

## Proof Of Concept's :

1. $200 Bounty Simple IDOR POC Bug Bounty

![[$200 Bounty _ Simple IDOR _ POC _ Bug Bounty _ @HacktivistsHub.mp4]]

2. [[$800 Bounty IDOR Complete Account Takeover Exploit POC]]

![[$800 Bounty __ IDOR __ Complete Account Takeover __ Exploit __ POC.mp4]]

3. [[$1000 bug bounty IDOR Insecure Direct Object References bug bounty poc hackerone]]

![[$1000 bug bounty _ IDOR _ Insecure Direct Object References _ bug bounty poc _ hackerone _.mp4]]

4. [[$2000 Bounty __ Simple IDOR __ POC __ Bug Bounty __ edalive.com]]

![[$2000 Bounty __ Simple IDOR __ POC __ Bug Bounty __ edalive.com.mp4]]

5. [[$3,000 Instagram delete highlight cover IDOR]]

![[[Bug Bounty] $3,000 Instagram delete highlight cover IDOR.mp4]]

6. [[IDOR Vulnerability to delete other's cart item]]

![[IDOR Vulnerability to delete other's cart item _ Bug Bounty POC.mp4]]

7. [[ign.com Self-star vulnerability]]

![[ign.com _ Self-star vulnerability Bug bounty Poc.mp4]]

8. Idor to Account Takeover __ IDOR POC ![[Idor to Account Takeover __ IDOR POC.mp4]]


































































