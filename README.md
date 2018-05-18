# Project 7 - WordPress Pentesting

Time spent: 10 hours spent in total

> Objective: Find, analyze, recreate, and document three vulnerabilities affecting an old version of WordPress

## Pentesting Report

1. User Enumeration
  - [ ] Summary: An Attack demonstrating how a persom cam become an accepted user afer an admin approves their comment allowing them to comment on any site
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: https://github.com/Ninjaguy87/Codepath-/blob/master/Priviledge%20Escalation%20Week%207.gif
  - [ ] Steps to recreate: 
        1. Comment on a post as a user
        2. Admin approve comment
        3. User can now comment freely without admin approval 
2. Stored XSS
  - [ ] Summary: A malicious script is injected into the site, which is then activated when the admin views the comment enabling a backdoor
    - Vulnerability types: Stored XSS Attack
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: https://github.com/Ninjaguy87/Codepath-/blob/master/XSS%20Stored%20Scripting%20Attack.gif
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
3. IDOR
  - [ ] Summary: The URL is maniuplated referencing a html file which reveals the version of word press being used
    - Vulnerability types: IDOR 
    - Tested in version: 4.2
    - Fixed in version: Fixable by Admin, hide or delete the object file
  - [ ] GIF Walkthrough: https://github.com/Ninjaguy87/Codepath-/blob/master/IDOR%20ReadMe.gif
  - [ ] Steps to recreate: 
          1. In the URL edit the code to look for the object we want
          2. change the url to http://wpdistillery.vm/readme.html
          3. click go and the version number and other relevant information about the wordpress site will be revealed




## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).


