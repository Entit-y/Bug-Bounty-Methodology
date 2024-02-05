1) Theres a request method called "HEAD" which can be used to retrieve header information of a requested resource

Here is an example  http t to a web resource using the "HEAD"  request
![[Pasted image 20231209002315.png]]

Here is the reponse from the web-server displaying the headers for the particular resource
![[Pasted image 20231209002349.png]]

Apache servers can serve files so when ever you test on an apache server, try putting ".htaccess" after the url to see if you can access the htaccess file
![[Pasted image 20231209002403.png]]


Mac's have a hidden file called ".DS_Store" that keeps track of the file system, you can try to add it on a url as well
![[Pasted image 20231209002410.png]]



2) After you identify an OS command injection vulnerability, it's useful to execute some initial commands to obtain information about the system. Below is a summary of some commands that are useful on Linux and Windows platforms:
![[Pasted image 20231209002422.png]]


Take note of the "multipart/form-data" inside the content-type header in an http (POST)request, it indicates that the request contains multiple parts that could be sending different types of data. Could be useful for file upload vulns
![[Pasted image 20231209002436.png]]

3) Be sure to use param-miner to check for supported headers, if the x-forwarded-for header is supported, it can be used to bypass a brute-force protection method that tells you to retry login after a certain amount of time because of too many incorrect tries.

4) when Brute forcing, make sure to use long passwords,  because an when an application determines that a username is correct, it goes on to process the password. if the password is wrong.. it'll take longer to process and determine if that passwd matches the username. that would cause a slight delay in the response which could indicate that the username is correct

(YOU CAN CHECK IF THIS METHOD WORKS ON AN APPLICATION BY SENDING THE LOGIN REQUEST TO THE REPEATER AND CONTINUOSLY INCREASING THE PASSWORD TO SEE IF THE TIME TAKEN IS LONGER ON LONGER PASSWORDS)

5) you can download an entire website using the "wget -m http://website.com" command

6) Try testing on non English sites more often because they not as tested on as the English site 

7) You can recognize JSON web tokens by the "eyJ" they begin with. anytime you encounter a string consistently containing "eyJ", you should put it in www.jwt.io to decode it

1) Attack registration forms more often, don't be shy

2) When ever you see a Hashtag(#) before a resource in a URL, its a Pointer for a potential DOM based [[Vulnerabilities/XSS|XSS]] attack vector. example: https://www.starbucks.co.jp/rewards/howtouse/#step1
3) The tech stack for an application isn't the same for all pages, different pages could used different technologies. make sure to check Wappalyzer consistently on relevant pages

4) When dealing with [[LFI]], just because a payload doesn't show in a browser doesn't mean it failed. if it wasnt blocked by a Waf, try making a *curl* request to the same endpoint with the payload:
```bash
curl https://target.com/../../../../../../../etc/passwd
```
12) in json, number values must not be put in quotes(Learned this the hard way) example:
```json
{
"price":"0"
}
```
wont work but:
```json
{
"price":0
}
```
works just fine
13) If you encounter a blog in an application, chances are its using wordpress. So make sure to fuzz for common wordpress endpoints like `/blog/wp-admin/`.
14) Pay attention to java script files on sensitive endpoints, for example java script files on a reset password page might disclose sensitive API endpoints or fields
15) Practice this lab more often and try to understand it better:
```http
https://portswigger.net/web-security/learning-paths/api-testing/api-testing-testing-for-server-side-parameter-pollution-in-the-query-string/api-testing/server-side-parameter-pollution/lab-exploiting-server-side-parameter-pollution-in-query-string#
```
16) 