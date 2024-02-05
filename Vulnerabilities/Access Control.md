[[Tags]] : #Testing #Bug 

## Description :

Access control is the application of constraints on who or what is authorized to perform actions or access resources. In the context of web applications, access control is dependent on authentication and session management:
- **Authentication** confirms that the user is who they say they are.
- **Session management** identifies which subsequent HTTP requests are being made by that same user.
- **Access control** determines whether the user is allowed to carry out the action that they are attempting to perform.
Broken access controls are common and often present a critical security vulnerability. Design and management of access controls is a complex and dynamic problem that applies business, organizational, and legal constraints to a technical implementation. Access control design decisions have to be made by humans so the potential for errors is high.

![[access-control.svg]]

## Testing :

- Access control vulnerabilities are best found manually, just pay attention to certain things that happen on the webapp
- Take note of every relevant page on the webapp, find out if it's a page that requires a user to sign in before gaining access to it.
- Take note of any request that contains an I.D or username or any other form of identifier.


## Proof Of Concept's :

1. $200 - Reset Password bypassing current Password - Response Manipulation Bug  ![[$200 - Reset Password bypassing current Password - Response Manipulation Bug Bounty POC - Professor 1.mp4]]
2. $360 bug bounty _ account takeover through reset password ![[$360 bug bounty _ account takeover through reset password 1.mp4]]
3. $500 Bounty for Improper Access Control _ Bug Bounty 2023 ![[$500 Bounty for Improper Access Control _ Bug Bounty 2023.mp4]]
4. $500 Bugbounty _ Open redirect in login and logout ![[$500 Bugbounty _ Open redirect in login and logout.mp4]]
5. 500 Dollars Bounty _ Lack Of Input Validation ![[500 Dollars Bounty _ Lack Of Input Validation.mp4]]
6. Accessing unauthorized _ Bug Bounty 2023 ![[Accessing unauthorized _ Bug Bounty 2023.mp4]]
7. Admin Panel Access _ P1 Bug _ Bug Bounty Program _ Bug Bounty POC 2023 ![[Admin Panel Access _ P1 Bug _ Bug Bounty Program _ Bug Bounty POC 2023.mp4]]
8. AT&T account takeover via rest password ![[AT&T account takeover via rest password _ bug bounty by mouhssine kassih 1.mp4]]
9. Broken Authentication and Session Management ![[Broken Authentication and Session Management 1.mp4]]
11. BUG BOUNTY 2023_ Email bypass ![[BUG BOUNTY 2023_ Email bypass.mp4]]
12. Clouddefenseai.com _ old token not expire lead full access ![[Clouddefenseai.com _ old token not expire lead full access.mp4]]
13. Email verification by pass on registration ![[Email verification by pass on registration 1.mp4]]
14. Email Verification Bypass POC ![[Email Verification Bypass POC 1.mp4]]
15. How to OTP Bypass, Response Manipulation and more ![[How to OTP Bypass, Response Manipulation and more 1 1.mp4]]
16. Open Redirect SAP _ NCIIPC GOV _ Bug Bounty POC ![[Open Redirect SAP _ NCIIPC GOV _ Bug Bounty POC 1 1.mp4]]
17. Password rest link  __ POC ![[Password rest link  __ POC.mp4]]
18. Session not expire after changing password ![[Session not expire after changing password.mp4]]
19. 
20. c
21. c
22. c