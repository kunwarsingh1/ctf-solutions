According to the bandit-0 page we have to login via ssh to get access to the shell of bandit-0 with usename bandit0 and server bandit.labs.overthewire.org on port 2220

So, we use the command ---
ssh bandit0@bandit.labs.overthewire.org -p 2220

after getting access to the shell we look into it using commands such as ----

bandit0@bandit:~$ ls
readme
bandit0@bandit:~$ cat readme 
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walkthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: <password>

and we get the password to the next level.
