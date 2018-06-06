# Detecting XSS using an IDS
This work focuses on the detection of XSS attack using intrusion detection system. Here attack signature is utilized to detect XSS attack. To test the usefulness and effectiveness of proposed work a proof of concept prototype has been implemented using SNORT IDS. It is observed that proposed system correctly detected XSS attack.

# Introduction to XSS
Cross Site Attacks are most common Network attacks across the web where we inject Payload (Malicious Code) on the client side to a website.
It’s a weakness found on poorly coded website which attacker exploits and tries. 
It uses victim's browser to deliver malicious script from a vulnerable site as vehicle. 
There are three actors in this attack (XSS) the attacker, the website and the victims can take use of JavaScript, Flash, VBScript and ActiveX. But mostly used is JavaScript.

# Procedure of XSS execution
1. Website database is infected through a payload by an attacker after submitting form with JavaScript Code.
2. Web page from the website is requested by a victim browser.
3. Victim's Browser is served the web page that was earlier requested by the victim with the payload attached to HTML body.
4. The payload will be executed inside the Victim's browser. Now attacker server will receive the victim's cookie. Victims cookie is extracted by the attacker. He uses victim’s cookie to make the HTTP request to the server.
5. After which attacker is granted request by the name of victim.

# Categories of XSS
1.Stored XSS: It take place when a target server stores the input from the user in the form of a message a database or visited log after this data becomes the part of website but instead of data user inputs a payload. When the stored payload is run locally, after which enables the malicious code that is saved as an data input by the user.

2.Reflected XSS: When a web application returns an error message, or any other response that comprises all input provided by the user immediately after user input was made.
