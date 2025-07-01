According to the bandit-1 page we have to login via ssh to get access to the shell of bandit-1 with username bandit1 and server bandit.labs.overthewire.org
on port 2220 with password from the previous level.


So, we use the command ---
ssh bandit1@bandit.labs.overthewire.org -p 2220

after getting access to the shell we look into it using commands such as ----

bandit1@bandit:~$ ls
-
bandit1@bandit:~$ cd ./-
-bash: cd: ./-: Not a directory
bandit1@bandit:~$ file ./-
./-: ASCII text
bandit1@bandit:~$ cat ./-
<password>

and we get the password to the next level.

