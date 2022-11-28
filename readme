# Project 7 - WordPress Pen Testing

Time spent: **4** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pen Testing Report

### 1. (Required) Vulnerability Name or ID

- [ ] Summary: Using a wordlist of common passwords and enumerating the users as we did previously, we can brute force passwords and retrieve login information for any user who chooses to use an insecure password.
  - Vulnerability types: Login Vulnerability
  - Tested in version: 4.2
  - Fixed in version: NA
- [ ] GIF Walkthrough: 
https://i.imgur.com/wM7cvRn.gif
- [ ] Steps to recreate: in kali terminal input wpscan --url http://wpdistillery.vm --wordlist /usr/share/wordlists/rockyou.txt --username admin
- [ ] Affected source code:
  - [Link 1](https://github.com/WordPress/WordPress/blob/4.2-branch/wp-login.php)
  
### 2. (Required) User enumeration using wpscan

- [ ] Summary: We can determine whether or not a user account exists on the WordPress install due to the different login errors. We can use wpscan to quickly enumerate all usernames since our install doesn't have a limit log attempt.
  - Vulnerability types: User Enumeration
  - Tested in version: 4.2
  - Fixed in version: NA
- [ ] GIF Walkthrough: https://i.imgur.com/pKOQcXN.gif
- [ ] Steps to recreate: in kali terminal input wpscan --url http://wpdistillery.vm --enumerate u
- [ ] Affected source code:
  - [Link 1](https://github.com/WordPress/WordPress/blob/4.2-branch/wp-login.php)

### 3. (Required) Shortcodes: can allow unclosed HTML elements in attributes

- [ ] Summary: Can allow malformed HTML elements to execute JS in the browser when creating, editing pages, or posts using plain text editor.
  - Vulnerability types: XSS
  -Tested in version: 4.2
  - Fixed in version: 4.2.5
- [ ] GIF Walkthrough: https://i.imgur.com/uvfxXxb.gif
- [ ] Steps to recreate: 1. Create a new page with any title you want 2. Inserty the following TEST!!![caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">XSS 💀</a> 3. View page and mouse over the alert to see the messages.
- [ ] Affected source code:
  - [Link 1](https://github.com/WordPress/WordPress/commit/f72b21af23da6b6d54208e5c1d65ececdaa109c8)


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with  ...
<!-- Recommended GIF Tools:
[Kap](https://getkap.co/) for macOS
[ScreenToGif](https://www.screentogif.com/) for Windows
[peek](https://github.com/phw/peek) for Linux. -->

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
    
