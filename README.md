# Cross-Site-Scripting

Xss is an abbreviation for cross site scripting. From  the title itself its clear 
xss is related to scripts to be precise its javascripts

xss is a very commoj attack found in web applications.'XSS' allows the attakers to insert
malicious code.

The attaker can inject his malicious script into a website,
and the browser just run's the code or script.

## Types of Xss
1.The First Attack is 'URL XSS' this means that the XSS wont stay on the page it will only get executed
if you have the malicious code in the URl and submit it the url 

2. The Second Attack is input fields:
Where ever you can insert data, it is very common, to be Xss vulnerable, for example say we found a site with a
Search engine, Now in the search box you enter 'hacker' now hit enter, when the page loads,if it says your data
like 'FOUND 100 Results for hacker' of now you can see its displaying out data on the page, now what if we can
execute code?there is no possible way to execute PHP code in this Attack, but  certainly is for HTML, javascript,
but be a aware this method, Also wont stay on the server, this is for eyes only

3. The third Attack, with this attack you will be able to INSERT data(code) and it will stay on the website:now there
are 2 kinds, it depends if we can execute PHP or HTML if we can inject PHP then we can inject HTML but not vice versa.

## Finding The XSS vulnerable Webiste

There are many techniques like:
- magic_quotes_gpc=ON bypass
- HEX encoding
- Obfuscation
- Trying around

## How does XSS work?

Cross-site scripting works by manipulating a vulnerable web site so that it returns malicious JavaScript to users. When the malicious code executes inside a victim's browser, the attacker can fully compromise their interaction with the application. 

## What are the types of XSS attacks?

   There are three main types of XSS attacks. These are:

   - Reflected XSS, where the malicious script comes from the current HTTP request.
   - Stored XSS, where the malicious script comes from the website's database.
   - DOM-based XSS, where the vulnerability exists in client-side code rather than server-side code.

## Xss used for following purpose ?

1. Used to access any data of user
2. Used for stealing login credential of user
3. Decline of the web site
4. Injecting different types of trojan in website

## Preventive measure of Xss

1. Do not trust any users input data
   - At the point where user input is received, filter as strictly as possible based on what is expected or valid input. 
2. Content Security Policy
   -  you can use Content Security Policy (CSP) to reduce the severity of any XSS vulnerabilities that still occur. 
3. Use appropriate response headers.
   - you can use the Content-Type and X-Content-Type-Options headers to ensure that browsers interpret the responses in the way you intend.
4. Set the HttpOnly flag
   - To mitigate the consequences of a possible XSS vulnerability, set the HttpOnly flag for cookies. If you do, such cookies will not be accessible via client-side          JavaScript. 
5. Use escaping/encoding
   - Use an appropriate escaping/encoding technique depending on where user input is to be used: HTML escape, JavaScript escape, CSS escape, URL escape, etc.
