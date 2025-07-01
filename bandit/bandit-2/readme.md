According to the bandit-2 page we have to login via ssh to get access to the shell of bandit-2 with username bandit2 and server bandit.labs.overthewire.org
on port 2220 with password from the previous level. After getting access to the shell we have to check the file named "spaces in this filename" and we would
get the password to the next level.


So, we use the command ---
ssh bandit2@bandit.labs.overthewire.org -p 2220

after getting access to the shell we look into it using commands such as ----

bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ file 
.bash_logout             .bashrc                  .profile                 spaces in this filename  
bandit2@bandit:~$ file spaces\ in\ this\ filename 
spaces in this filename: ASCII text
bandit2@bandit:~$ cat spaces\ in\ this\ filename 
<password>
bandit2@bandit:~$ 


and we get the password to the next level.
