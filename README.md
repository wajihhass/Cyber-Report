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
### Horizontal Rule

You can add a Horizontal Rule by putting three underscores, asterisks, or minus signs together one line alone

Syntax Example:

```
___

or

---

or

***
```

Real Example:

***

***

### Phrase emphasis

You can make text italic by putting an asterisk or underscore before and after your statement

Syntax example:

```
*This would be italic if it wasn't in a code block*

_This would also be Italic because of the underscores_
```

Real Example:

Look, *this is Italic*, isn't that cool?

You can also make text bold by putting two asterisks or underscores around it

Syntax Example:

```
**This would be BOLD because this statement has two asterisks wrapped around it**

__This would be BOLD too__
```

Real example:

**BOLD TEXT**

Using a combination of underscores and asterisks you can make text bold and italic

Syntax example:

```
**Only Bold, _Bold and Italic,** Only Italic_
```

Real Example:

**Only Bold,** **_Bold and Italic,_** _Only Italic_

To put a line through text you can wrap it with two tildes

Syntax example:

```
~~This is wrong~~
```

Real Example:

~~This is wrong~~

***

### Listing items

To list items in an unordered list you can put a minus sign followed by a space in front each item you want to list. Each item should have its own individual line, as seen in my example.

Syntax example:

```

- Item One
- Item Two
- Item Three

```

Real example:

- Item One
- Item Two
- Item Three

For an ordered list you can just put them numbers with a period after in front of each item and it will automatically format the list for you

Syntax Example:

```

1. Item

2. Item

3. Item

```

Real Example:

1. Item

2. Item

3. Item


***

### Adding links to your Markdown File

Often times you will want to put links in your notes to other content.

To do this, you put the text you want to add a link to in square braces "[Click me to go to google.com]" followed by the URL in parentheses "(www.google.com)". After the URL in the parentheses you can add text to your link that will appear when a user hovers over the link by adding that message in quotations after your link like this: (google.com "This is a link to google")

Syntax example:

```
Why don't you [Click me to go to google.com](google.com "This link will take you to google")
```

Real example:

Why don't you [Click me to go to google.com](https://www.google.com/ "This link will take you to google")

***

### Tables

You can add tables to your Markdown by using hyphens and straight lines as seen below. By using colons too you can change how the text formats in the columns also seen below with the centered and right-alighed text

Syntax Example:

```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
```

Real Example:

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

***

### Block Quotes

You can put test in a Block Quote by putting a '>' at the beginning of the line, this will make that line stand out more. Using block quotes is good because it wraps text, unlike code and syntax highlighting

Syntax example:

```
> This text will appear in a block quote
```


Real Example:

> This text will appear in a block quote

***

### Adding a Youtube Video:

To add a youtube video it is best to use HTML because then you can add a border and image sizing that you would not have if you tried to add a video in pure Markdown

Syntax Example:

```
<a href="https://www.youtube.com/watch?v=6A5EpqqDOdk" target="_blank"><img src="http://img.youtube.com/vi/6A5EpqqDOdk/0.jpg" alt="A link to the Markdown Tutorial Video" width="240" height="180" border="10" /></a>
```

Real Example:

<a href="https://www.youtube.com/watch?v=6A5EpqqDOdk" target="_blank"><img src="http://img.youtube.com/vi/6A5EpqqDOdk/0.jpg" alt="A like to the Markdown Tutorial Video" width="240" height="180" border="10" /></a>

***

### Inline HTML

You can also add raw HTML into your Markdown and it will work most of the time, as seen above with the Youtube video

***

### Adding Images

You can add an image by using this syntax:

```
![alt tag](https://github.com/CodyNicholson/CodyNicholson.github.io/blob/master/images/topBanner.jpg)
```

With a link to your image passed as the parameter

Real Example:

![alt tag](https://github.com/CodyNicholson/CodyNicholson.github.io/blob/master/images/topBanner.jpg)
