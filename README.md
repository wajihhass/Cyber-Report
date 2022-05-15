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
#### 1. it’s crucial that you turn off HTTP TRACE support on all web servers. An attacker can steal cookie data via Javascript even when document.cookie is disabled or not supported by the client

#### 2. Framework Security
Fewer XSS bugs appear in applications built with modern web frameworks. These frameworks steer developers towards good security practices and help mitigate XSS by using templating, auto-escaping, and more. That said, developers need to be aware of problems that can occur when using frameworks insecurely such as:

##### a. escape hatches that frameworks use to directly manipulate the DOM

##### b. React’s dangerouslySetInnerHTML without sanitising the HTML

##### c. React cannot handle javascript: or data: URLs without specialized validation

##### d. Angular’s bypassSecurityTrustAs* functions

##### e. Template injection

##### f. Out of date framework plugins or components

#### 3. Each variable in a web application needs to be protected. Ensuring that all variables go through validation and are then escaped or sanitized is known as perfect injection resistance. Any variable that does not go through this process is a potential weakness


***

***
### Q4. Are there notable examples of this type of attack in the news?

The most common example can be found in bulletin-board websites which provide web based mailing list-style functionality.

***
# Cybersecurity Current Event Report

***
### Q1. What type of attack was this?

The hacking incidents during the 2016 presidential race between Donald Trump and Hillary Clinton. 

*** 
 ### Q2. How was the vulnerability discovered?
The FBI contacts the Democratic National Committee’s help desk, cautioning the IT department that at least one computer has been compromised by Russian hackers. May-June 2016 - The hackers steal thousands of emails from the DNC server and begin to conceal their efforts. 

*** 

### Q3. How were the attackers able to exploit the vulnerability
June 14, 2016 - The Washington Post reports hackers working for the Russian government accessed the DNC’s computer system, stealing oppositional research on Trump and viewing staffers’ emails and chat exchanges. The Kremlin, however, denies that the government was linked to the hack and a US official tells CNN that investigators have not yet concluded that the cyberattack was directed by the Russian government.
***

### Q4. Were there security measures that could have been taken in order to prevent this attack?




***
