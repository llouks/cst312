# 312codepath, 
CodePath Week 7 Assignment
Logan Louks
11/6/2018

# Directions:
For this week's assignment, discover and demonstrate similar proofs-of-concept for at least an additional three and (up to five) exploits affecting an older version of WP. Submit the write-ups and walkthroughs via Github. Check out the Submitting Assignments page for more details. Be sure to include a README.md based on this README template containing a small writeup and GIF walkthroughs of each exploit.

# Exploits

# Project 7 - WordPress Pentesting

Time spent: **3.5** hours spent in total

Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report
    
1. CVE-2017-1000600

Summary: WordPress version 4.9 contains a CWE-20 Input Validation vulnerability in thumbnail processing that can result in remote code execution. This attack appears to be exploitable via thumbnail upload by an authenticated user and may require additional plugins in order to be exploited however this has not been confirmed at this time. This issue appears to have been partially, but not completely fixed in WordPress 4.9	
  
Vulnerability types:
Confidentiality Impact - Partial (There is considerable informational disclosure.)
    
Integrity Impac - Partial (Modification of some system files or information is possible, but the attacker does not have control over what can be modified, or the scope of what the attacker can affect is limited.)

Availability Impact	- Partial (There is reduced performance or interruptions in resource availability.)

Access Complexity -	Low (Specialized access conditions or extenuating circumstances do not exist. Very little knowledge or skill is required to exploit. )

Gained Access -	None
    
Tested in version: 4.9

Fixed in version:  
  
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code: 
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    https://www.cvedetails.com/cve/CVE-2017-1000600/
    

2. CVE-2009-2762

Summary: wp-login.php in WordPress 2.8.3 and earlier allows remote attackers to force a password reset for the first user in the database, possibly the administrator, via a key[] array variable in a resetpass (aka rp) action, which bypasses a check that assumes that $key is not an array.

Vulnerability types: Bypass

Confidentiality Impact: Partial (There is considerable informational disclosure.)

Integrity Impact: Partial (Modification of some system files or information is possible, but the attacker does not have control over what can be modified, or the scope of what the attacker can affect is limited.)

Availability Impact: Partial (There is reduced performance or interruptions in resource availability.)
Access Complexity: Low (Specialized access conditions or extenuating circumstances do not exist. Very little knowledge or skill is required to exploit. )

Authentication: Not required (Authentication is not required to exploit the vulnerability.)

Gained Access: None

Tested in version:2.8.3

Fixed in version: 2.8.4

  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


3. CVE-2007-2821

Summary: SQL injection vulnerability in wp-admin/admin-ajax.php in WordPress before 2.2 allows remote attackers to execute arbitrary SQL commands via the cookie parameter.

Vulnerability types: Exec, Code, Sql

Confidentiality Impact:	Partial (There is considerable informational disclosure.)

Integrity Impact: Partial (Modification of some system files or information is possible, but the attacker does not have control over what can be modified, or the scope of what the attacker can affect is limited.)
Availability Impact	Partial (There is reduced performance or interruptions in resource availability.)
Access Complexity	Low (Specialized access conditions or extenuating circumstances do not exist. Very little knowledge or skill is required to exploit. )

Authentication: Not required (Authentication is not required to exploit the vulnerability.)

Gained Access: User

Tested in version: 2.2

Fixed in version:  2.3

  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

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
