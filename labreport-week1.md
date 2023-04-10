# Remote Access and FileSystem
## Step 1 *Installing VScode*
Go to the link provided here [link](https://code.visualstudio.com/) and follow the instructions on the website to install different versions of VScode on Windows/MacOS.
![Image](screenshot1.png)
***
## Step 2 *Remotely Connecting*
* First you need to get your course-specific account here: [link](https://sdacs.ucsd.edu/~icc/index.php). Change the password following instructions on website.
* Open a terminal in VScode (use the Terminal → New Terminal menu option). Then type in `$ ssh cs15lsp23zz@ieng6.ucsd.edu` with the "zz" replaced by your own cse15L course account. When you see messages:
```
The authenticity of host 'ieng6.ucsd.edu (128.54.70.238)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
Type in "yes" to continue connecting.
* After typing yes, you should be seeing a prompt asking for your password, type in the password of your course-specific account and press enter.
* You are successfully connected if you see these lines in your terminal:
```
ssh cs15lsp23fh@ieng6.ucsd.edu
(cs15lsp23fh@ieng6.ucsd.edu) Password: 
(cs15lsp23fh@ieng6.ucsd.edu) Password: 
Last failed login: Sun Apr  9 22:25:18 PDT 2023 from cpe-66-75-229-17.san.res.rr.com on ssh:notty
There was 1 failed login attempt since the last successful login.
Last login: Wed Mar 15 15:42:38 2023 from 100.81.39.153
============================ NOTICE =================================
Authorized use of this system is limited to password-authenticated
usernames which are issued to individuals and are for the sole use of
the person to whom they are issued.

Privacy notice: be aware that computer files, electronic mail and 
accounts are not private in an absolute sense.  You are responsible
for adhering to the ETS Acceptable Use Policies, which you can review at:
https://blink.ucsd.edu/faculty/instruction/tech-guide/policies/ets-acceptable-use-policies.html
=====================================================================

*** Problems, Suggestions, or Feedback ***
    
    For help requests, please create a ticket at:
    https://support.ucsd.edu/its 

    You may also report issues, suggestions, or feedback by e-mailing root on any system:
    mail -s "Your subject here" root
    Type your message - Ctrl+D to send
    
*** Access our Linux ssh terminals or remote desktops via a web browser at: ***
    https://linuxcloud.ucsd.edu

    All accounts must be enrolled in Duo for access. No VPN required.


-------------------------------------------------------

quota: Cannot resolve mountpoint path /home/linux/ieng6/.snapshot/hourly.2023-04-02_2001: Stale file handle
quota: Cannot resolve mountpoint path /home/linux/ieng6/.snapshot/hourly.2023-04-04_2001: Stale file handle
quota: Cannot resolve mountpoint path /home/linux/ieng6/.snapshot/hourly.2023-04-04_1601: Stale file handle
Hello cs15lsp23fh, you are currently logged into ieng6-201.ucsd.edu

You are using 0% CPU on this system

Cluster Status 
Hostname     Time    #Users  Load  Averages  
ieng6-201   22:25:01   13  1.80,  1.78,  1.20
ieng6-202   22:25:01   11  3.25,  3.20,  3.25
ieng6-203   22:25:01   8   0.04,  0.13,  0.18

 
Sun Apr 09, 2023 10:25pm - Prepping cs15lsp23
```
![Image](screenshot2.png)
***
## Step 3 *TryingSomeCommands*
There are a lot of commands that we can use in the terminal, here are some basic ones:
* `cd ~`
* `cd`
* `ls -lat`
* `ls -a`
* `ls <directory>` where `<directory>` is `/home/linux/ieng6/cs15lsp23/cs15lsp23abc`, where the `abc` is one of the other group members’ username
* `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/`
* `cat /home/linux/ieng6/cs15lsp23/public/hello.txt`
![Image](screenshot3.png)
***




