# Project 8 - Pentesting Live Targets

Time spent: **7** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection
![SQL Injection](https://raw.githubusercontent.com/jamesw8/pentesting-live-targets/master/SQL_Injection.gif)

In the salesperson directory, it uses the id parameter in the URL to perform SQL queries without sanitizing. In the GIF, we can enter an AND clause and if we set it to a false boolean value, then we will be redirected to the directory as Blue makes sure to redirect for ids that are not found.

Vulnerability #2: Session Hijacking/Fixation
![Session Hijacking](https://raw.githubusercontent.com/jamesw8/pentesting-live-targets/master/Session_Hijacking.gif)

Using two different browsers, one acting as a normal user and one as a staff user, changing the session id on the normal user's browser to the staff user's session will give access to the staff menu.


## Green

Vulnerability #1: User Enumeration
![User Enumeration](https://raw.githubusercontent.com/jamesw8/pentesting-live-targets/master/user_enumeration.gif)

The difference between the failure and failed class determines if the user for the login attempt actually exists.

Vulnerability #2: Cross-Site Scripting
![Cross-Site Scripting](https://raw.githubusercontent.com/jamesw8/pentesting-live-targets/master/XSS.gif)


Entering the name `<script>alert('James found the XSS!');</script>` in the contact/feedback form will execute the script when the staff views the feedback. As you can see, a previous student added a script to redirect to Google so my script will not be able to run. It would, however, execute in the absence of a preceding redirect.


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work

