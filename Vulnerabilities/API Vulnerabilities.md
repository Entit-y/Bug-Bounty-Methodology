[[Tags]] : #Testing #Bug 

## Description :

API vulnerabilities are bugs that that affect the API(Application programming interface) of a Web application or service. These bugs can expose sensitive data, compromise user privacy or allow unauthorised access to a system. Some common API vulnerabilities include:
- Injection attack vectors
- Authorization flaws
- Authentication issues
- Sensitive data exposure
- Rate limiting bypass
- Input validation
- Denial of service(DoS)
## Testing :

- Gather information on the API, identify and document API endpoints by analyzing the application's documentation and web-traffic.
- Understand the authentication mechanisms like how the API handles user authentication(e.g., API Keys, OAuth tokens)
- Review the API's official documentation for security related information including authentication, authorization and data protection mechanisms. Be sure to look for deprecated or outdated features that might introduce vulnerabilities

- When testing for API Vulns,  check if the application is following best practices for API security, check if they:
	- Secure Thier documentation if They don't intend their API to be publicly accessible.
	- Ensure their documentation is kept up to date.
	- Apply an allowlist of permitted HTTP methods.
	- Validate that the content type is expected for each request or response.
	- Use generic error messages to avoid giving away information that may be useful for an attacker.
	- Use protective measures on all versions of their API, not just the current production version.

## Proof Of Concept's :

1. Found AWS API Keys using “Trufflehog” & Validated them using [[Enumerate-iam]] tool _ Bug Bounty PoC ![[Found AWS API Keys using “Trufflehog” & Validated them using “enumerate-iam” tool _ Bug Bounty PoC 1.mp4]]
2. GOOGLE API key leaked Vulnerability on licious  _ P5 BUG HackerOne _ Bug bounty POC _ 2023 ![[GOOGLE API key leaked Vulnerability on licious  _ P5 BUG HackerOne _ Bug bounty POC _ 2023.mp4]]
3. Swagger API to XSS on IBM _ Bug Bounty POC ![[Swagger API to XSS on IBM _ Bug Bounty POC.mp4]]
















