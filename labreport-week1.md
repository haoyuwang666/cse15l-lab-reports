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
* You are successfully connected if you see this line in your terminal:

    `Hello cs15lsp23fh, you are currently logged into ieng6-201.ucsd.edu`

![Image](screenshot2.png)
***
## Step 3 *Trying Some Commands*
There are a lot of commands that we can use in the terminal, here are some basic ones:
* `cd ~` Change directory to home directory(a directory where a user's files are stored)
* `cd` cd with no argument provided goes to home directory as well
* `ls -lat` showing all the files within the current directory of our Linux system in the descending order of their time created
* `ls -a` Type the ls -a command to list files or directories including hidden files or directories
* `ls <directory>` where `<directory>` is `/home/linux/ieng6/cs15lsp23/cs15lsp23abc`, where the `abc` is one of the other group members’ username. Type the ls [directory path here] command to list the contents of another directory. This shows the contents in your remote server
* `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/` copy the hello.txt file in your directory
* `cat /home/linux/ieng6/cs15lsp23/public/hello.txt` paste the hello.txt file in your directory
![Image](screenshot3.png)
***




