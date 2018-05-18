# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. User Enumeration
  - [ ] Summary: An Attack demonstrating how a persom cam become an accepted user afer an admin approves their comment allowing them to comment on any site
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: https://giphy.com/gifs/40bI4vFdon1dsSD1wv
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
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
          1. In the URL edit the code to look for the object we want
          2. change the url to http://wpdistillery.vm/readme.html
          3. click go and the version number and other relevant information about the wordpress site will be revealed



## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
