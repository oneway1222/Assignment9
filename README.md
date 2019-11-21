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

Vulnerability #2: __________________


## Green

Vulnerability #1: __________________

Vulnerability #2: __________________


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work

