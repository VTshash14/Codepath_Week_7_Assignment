# CyberSecurity Week 7 Assignment

# Week 7 Project: WordPress vs. Kali

Time spent: 15 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1\. (Required) WordPress <= 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS)
- [x] Summary: 
- Vulnerability types: XSS
- Tested in version: 4.2
- Patch version: 4.2
- [x] GIF Walkthrough:<img src='https://i.imgur.com/3hajE9h.gif' title='GIF Walkthrough' width='' alt='GIF Walkthrough' /> 
- [x] Steps to recreate: Go to the comments section of the page. Enter the following script in the comments: <script>while(1){alert(document.cookie);}</script>
- [x] Affected source code:
- [Link 1](https://compsecurityconcepts.wordpress.com/tag/cross-site-scripting/)

2\. (Required) WordPress 4.2.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeded
- [x] Summary: 
- Vulnerability types: XSS and Inject
- Patch version: 4.2.2
- Fixed in version: 4.2.13

- [x] GIF Walkthrough:<img src='https://i.imgur.com/swNTjs4.gif' title='GIF Walkthrough' width='' alt='GIF Walkthrough' /> 
- [x] Steps to recreate: 
- Choose an youtube video that you would like to embed into the post
- Add "[embed src=‘https://youtube.come/embed/12345\x3csvg onload=while(1){alert(document.cookie};\x3e’][/embed]" with the URL
- Post the post
- You will recieve an error message and be redirected to the images source.
- [x] Affected source code:
- [Link 4](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)

3\. COULD NOT COMPLETE THE LAST ONE. WAS HAVING PROBLEMS WITH WORDPRESS AND TERMINAL.



GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Notes
This assignment was extremely difficult. One of the most stressful things. I had to restart the process of installing the software atleast 5 times. Even after I got two to work I had problems with the last one.

## License

Copyright [2017] [Shashank Shinde]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
