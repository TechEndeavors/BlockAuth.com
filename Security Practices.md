##Security Practices
Security is paramount with this system. We need to worry about regular server security as well as account hijacking. 

###Server security
* All servers need to have a firewall in place. SSH is always at a higher port running fail2ban. Also, authentication requires a SSH key AND a username and password to login, with the root account disabled. Raising to root permissions uses sudo and requires the user to re-enter their password
* If it’s a database server, then the DB port should only allow access to the IP address of other DB servers and the web server. 
* Web servers only allow access to the whitelist of Cloudflare IP’s. 
* No servers are hosted at low-end VPS’s
* Backups are created on the server itself, encrypted, and transferred to S3 for storage

###Data Security
* All data at rest is encrypted with a public key that resides on the server before being transferred to S3. 

###Account Hijacking prevention
Users have access to enable several-factor-authorization - They can enable Authy, require a TXT message or email. 
Security paranoid levels can be adjusted to different paranoia levels in three categories

*Logins*
* Casual - Just requires username and password. Password resets require confirmation email
* Cautious - Regularly requires username and password. If login occurs from an IP in an area significantly far away from the user, it requires 2fa. 
* Nervous - Regularly requires username and password. If login occurs from a non-whitelisted IP address, it requires 2fa. If login occurs from an IP in an area significantly far away from registered location, it also requires answering a security question. 
* Paranoid - All logins require username, password, and 2fa. If login occurs from a non-whitelisted IP address, also requires answering security questions. 
* Tin Foil hat - All logins require username, password, 2fa, and SMS verification. If login occurs from a non-whitelisted IP address, also requires answering security questions. 


*Password Resets*
* Casual - Password resets is delivered via email
* Cautious - Password reset requires answering a security question. Reset code is delivered via email or txt according to what the user requests. Notification is sent to the other medium
* Nervous - To reset the password, the user stays on the password reset webpage while Password reset requires receiving an automated phone call and answering some multiple-choice security questions. Upon success, the user is given a code they type in. If that code is correct, they can reset their password. Notification is sent to txt and email.
* Paranoid - Password reset is only possible with an automated video interview where they are asked the multiple choice security questions. A support person will review the request. When the request has been approved, they will receive an email and txt message asking them to click a link to initiate a phone call that tells them the password reset code. 
* Tin Foil hat - Password reset can be initiated with same video interview process, but the password reset code is sent via postal mail. 

###Examples of security questions
* Which of these 5 foods do you like the most? (from a pool of 20 choices)
* Which of these 5 scary animals do you like the least? (from a pool of 20 choices)
* Which of these 5 instruments do you like hearing the most in a song? (from a pool of 20 choices)
* Which of these 5 things do you enjoy the most in your spare time? (from a pool of 20 choices)
* Which of these 5 vacation destinations looks the most enjoyable to you? (from a pool of 10 choices)



