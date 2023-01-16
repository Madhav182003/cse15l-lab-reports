# Lab Report - 1

---

This is a tutorial for 15L students on how to log into the course specific account on *ieng6* and remotely connect to the server from your computer.

The tasks to be performed are -

* Installing VSCode
* Remotely Connecting
* Trying some Commands

## Step-1 Installing VSCode

Use the folloiwing link to go to the VSCode website [Link](https://code.visualstudio.com/), and follow the on screen instructions to download and install it on your computer.

There are different versions available for all major OS like windows, mac etc.

When VSCode is installed the following window should open.

![Image](https://user-images.githubusercontent.com/122562063/212574161-14b34b3d-5b00-4947-9d1f-d7c8d48e767e.png)

## Step-2 Remotely Connecting

To continue with this step you first need to look up your CSE15L specific account here-  [Link](https://sdacs.ucsd.edu/~icc/index.php)

It will take you to the following screen

![Image](https://user-images.githubusercontent.com/122562063/212574376-fa16c562-36f5-49f4-b20f-5dd47c098562.png)

Enter your information and click submit.

You will then be redirected to the following screen - 

![Image](https://user-images.githubusercontent.com/122562063/212574449-b08a64a7-eaa0-4aff-b8c7-6e8541f42e14.png)

Here you can see your Course sepcific username. Click on it and change your password by following the on screen instructions.

After you are done changing and password and noting down your username, open a terminal in VSCode.

Then use the *ssh* command given below but replace the **zz** with the the letters in your own username to connect to the server.

    $ ssh cs15lwi23zz@ieng6.ucsd.edu

Then enter the password that you just changed.

Once logged in a screen like the one below will appear

![Image](https://user-images.githubusercontent.com/122562063/212586523-19066250-2e68-497f-b2a7-b4b711dd916e.png)

Now your terminal is connected to a computer in the CSE Basement and commands run by you will run on that computer.

## Trying some Commands

Now you can try running some commands like **cd, ls, pwd, mkdir, and cp** on your computer and the remote computer.

Below are some specific commands to try-

* cd ~
* cd
* ls -lat
* ls -a
* ls <directory> where <directory> is /home/linux/ieng6/cs15lwi23/cs15lwi23abc, where the abc is one of the other group members’ username
* cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lwi23/public/hello.txt

![Image](https://user-images.githubusercontent.com/122562063/212587475-87f75f86-3ab8-4740-9440-44429ffe23b0.png)
  


To log out you can use the following-
  
* Control-D
* run the command **exit**















