# windows su
Elevate windows cmd beyond normal admin - to the `system` account

# Installation:
0. Get and install sysinternals full package or just psexec. It's required for this script.
1. Download the .bat script
2. Put it in your PATH, for example:
  - put in C:\Windows\system32
  - check your PATH and select one of these
  - create new directory and put it there, add it to PATH
3. If you want the command to be different, just rename the script

# Why
This will pop up new cmd window with NT\System user. That permission level is beyond normal admin and in 99% cases when you think you need it, you are likely doing something wrong. But if you **really** need it, here it is.

# Usage

Just type in `su`, you will be prompted by UAC, accept it, and new window will pop out. To verify everything worked, type `whoami` command. You should get NT\System account, instead of your standard admin.

Note, it's still not as "root" as linux `su`, but its still closer than your avarage shell as admin

# Kudos
[This](https://stackoverflow.com/questions/7044985/how-can-i-auto-elevate-my-batch-file-so-that-it-requests-from-uac-administrator/12264592#12264592) stack overflow anwser. I just put the thing here so it's easier to find on gh.