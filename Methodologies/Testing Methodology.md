
## [[Vulnerabilities/XSS|XSS]]:
When testing for xss, make sure you check for reflected input in cookies. Some applications store user input in their cookies which could be reflected in the DOM. 
	Reference:
	[[Cookie Based XSS _ Bug Bounty Poc 1.mp4]]

## [[API Vulnerabilities#Testing]]:
Use burp to locate all API calls made on the webapp, take note of every parameter sent by the client or received by the server. and insert them in API requests.

With API testing, I think the main goal is to try to cause an error of some sort. the error message may give some insight on what is going on in the backend to further build the exploit.
		`note: not all errors will give a well articulated error message, this is a security measure to make a hackers job difficult by giving less hints. make sure to analyse the steps you took to cause that error if this should happen`