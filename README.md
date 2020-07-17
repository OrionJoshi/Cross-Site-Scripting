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
