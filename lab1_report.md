# Lab Report 1
---
**This is a tutorial for logging into your course specific account on ieng6**

## Installing Visual Studio Code
Go to [link](https://code.visualstudio.com/) and 
follow the instructions to download vscode on your computer.

When it is installed, you should be able to open a window that looks 
like this (it might look slightly different. That's ok!):
![Image](vscode.png)

Note: I didn't have to do this step (of installing vscode) as I already had it installed on my system.

## Remotely connecting
The goal here is to use the vscode terminal
to connect to a remote computer over the Internet and then do work there.

If you’re on Windows: install git from the site:
[git for windows](https://gitforwindows.org/)

After that, use the steps in the following link to use git bash in vscode:
[bash on vscode](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994)

Note: I didn't install/use git (I already had it installed on my system) because I'm on MacOS.

Use the Terminal → New Terminal menu option to open a terminal on vscode where you can use ssh as follows (replace zz with the letters in your own course specific account)

`$ ssh cs15lsp23zz@ieng6.ucsd.edu`

Since this might be the first time you’ve connected to this server, you will probably get a message like this:

`ssh cs15lsp23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?`


Type `yes` and press enter, then give your password. It should look like this after you are logged in:

`# On your client
⤇ ssh cs15lsp23zz@ieng6.ucsd.edu
The authenticity of host 'ieng6-202.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
Password: `

![Image](remote_connection.png)

Now your terminal is connected to a computer in the CSE basement, and your commands will be run on that computer! So your computer can be considered as the client and the computer in the CSE basement as the server.

## Trying some commands
Try running the commands cd, ls, pwd, mkdir, cat and rmdir a few times on your terminal (after ssh-ing)

`cd`

`ls`

`pwd`

`mkdir new_directory`

`rmdir new_directory`

`cat /home/linux/ieng6/cs15lsp23/public/hello.txt`

![Image](commands.png)

To log out of the remote server in your terminal, do:
* Ctrl-D
or
* Run the command exit
You can also open more terminals in VSCode using the + button at the top of the terminal.

If in doubt or if you encounter an error in any of the steps, just ask someone!

You have finished the tutorial. Congratulations!
