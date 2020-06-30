(**WARNING: ORANGEOS IS NOT UPLOADED OR RELEASED TO THIS REPO YET SO THINGS IN THIS README FILE MAY BE INVALID UNTIL FILES ARE UPLOADED**)


# Welcome to Orange OS!
Hello and thanks for your interest in Orange OS! I will give you a full walkthrough of my Python program in this README file...
## What is Orange OS?
**OrangeOS is not an Operating System** (I was using a name of a now-discontinued project for this because I could not think of a name for this). OrangeOS is a small python program which provides a commandline interface on your Windows PC. This command line interface (in version 1 at least) is very primitive and should not replace your regular cmd.exe or powershell.exe. 

Still with us? Good.
## The setup process
When you download a version of Orange OS for the first time, you will be met with a setup script. 
*PLEASE LAUNCH THE WINDOWS COMMAND SCRIPT BEFORE THE PYTHON SCRIPT! The Python Script depends on the things the command script does and will not work without it.*
Setup is pretty simple, the command script extracts the base system files into a directory called C:\OrangeOS (WARNING: If this directory exists, it will (after warning you) DELETE it, so rename the directory or move the files out of it). Then it extracts the Recovery Environment to C:\OrangeOS_Recovery, you can launch the recovery environment if your installation of OrangeOS has become corrupted.
After extracting the base system and the recovery environment (and doing a few other things, like making you install Python if you don't have it already), setup then automatically switches to the Python script. This script takes care of things such as creating a new user (IMPORTANT STEP!! OrangeOS REQUIRES a user or you cannot access it!) and setting a password (THE PASSWORD CANNOT BE BLANK!!! Or the login system will have trouble and MAY NOT log you in)
After setup, you are "booted" into your new installation. 

## "Boot"
You will see this on every boot: (for this example, let's say we created a user called "test")
```
[Starting] Starting shell...
Please Log In.

Username? test
test's Password? 
```
(For the password, your input isn't shown for security reasons)
and after entering the username and password of your newly created user, you are booted into the shell. It looks like this:
```
test [C:\OrangeOS\test]: _
```

Now, lets talk about commands.

##Commands

By default, OrangeOS comes with the BARE commands. These are: **making a user, deleting a user, changing your password, exit and reboot (which is like a log out)**
That's all you get, no help, nothing.
BUT If you go to this GitHub repo, you should see a folder called "OptionalCommands". Inside the folder are HUNDREDS of extra commands with their own instructions, so follow them!

##Security

**OrangeOS is NOT secure.** Granted, we have a login manager and hash passwords BUT, this version of OrangeOS comes uncompiled (Second version comes compiled) so it is EASY for a person who knows Python to change the shell's and the command's code and make it avoid login.
We are trying to make v2 compiled so that it isn't as easily editable.

##Feedback and commits
We would LOVE it if you could give us feedback and actually commit to our work and edit it. This is just a random hobby of mine during quarantine and it would be great if you could contribute to it.

Thanks!
OrangeOS Dev Team
