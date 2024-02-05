- [ ] Check and note down all cookie parameters for the application
- [ ] check to see if any cookie values are being reflected anywhere on the application
	If a cookie value is being reflected on the application, test for [[Vulnerabilities/XSS|XSS]] by inspecting the DOM and crafting payload to be used. use the browser cookie storage or the cookie editor extension to input the payload
- [ ] check to see if any input values are being stored in the cookies
	To know whether an input value is being directly stored in the cookie, give an input that is stored on the DOM, close and reopen the same website and see if that same input is returned. If this is true, test for [[Vulnerabilities/XSS|XSS]] by inputting a payload from inspecting the DOM to craft it