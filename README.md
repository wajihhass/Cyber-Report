# Cyber-Report
# Cyber Strategies Report


   ## Cross Site Scripting (XSS)



***
### Q1. Specifically, how is this type of attack conducted?

Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted websites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user. Flaws that allow these attacks to succeed are quite widespread and occur anywhere a web application uses input from a user within the output it generates without validating or encoding it.

***

***
### Q2. What are the biggest risks from this type of attack?

An attacker can use XSS to send a malicious script to an unsuspecting user. The end user’s browser has no way to know that the script should not be trusted, and will execute the script. Because it thinks the script came from a trusted source, the malicious script can access any cookies, session tokens, or other sensitive information retained by the browser and used with that site. These scripts can even rewrite the content of the HTML page
***
***
### Q3. How can this type of attack be defended against?
1. it’s crucial that you turn off HTTP TRACE support on all web servers. An attacker can steal cookie data via Javascript even when document.cookie is disabled or not supported by the client

2. Framework Security
Fewer XSS bugs appear in applications built with modern web frameworks. These frameworks steer developers towards good security practices and help mitigate XSS by using templating, auto-escaping, and more. That said, developers need to be aware of problems that can occur when using frameworks insecurely such as:

a. escape hatches that frameworks use to directly manipulate the DOM

b. React’s dangerouslySetInnerHTML without sanitising the HTML

c. React cannot handle javascript: or data: URLs without specialized validation

d. Angular’s bypassSecurityTrustAs* functions

e. Template injection

g. Out of date framework plugins or components

3. Each variable in a web application needs to be protected. Ensuring that all variables go through validation and are then escaped or sanitized is known as perfect injection resistance. Any variable that does not go through this process is a potential weakness


***

***
### Q4. Are there notable examples of this type of attack in the news?

The most common example can be found in bulletin-board websites which provide web based mailing list-style functionality.

***
# Cybersecurity Current Event Report

***
### Q1. Specifically, how is this type of attack conducted?

Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted websites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user. Flaws that allow these attacks to succeed are quite widespread and occur anywhere a web application uses input from a user within the output it generates without validating or encoding it.

*** What type of attack was this?
