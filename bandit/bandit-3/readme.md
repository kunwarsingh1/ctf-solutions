According to the bandit-3 page we have to login via ssh to get access to the shell of bandit-3 with username bandit3 and server bandit.labs.overthewire.org
on port 2220 with password from the previous level. After getting access to the shell we have to check the password stored in a hidden file in the inhere
directory


So, we use the command ---
ssh bandit3@bandit.labs.overthewire.org -p 2220

after getting access to the shell we look into it using commands such as ----

bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -la
total 12
drwxr-xr-x 2 root    root    4096 Apr 10 14:23 .
drwxr-xr-x 3 root    root    4096 Apr 10 14:23 ..
-rw-r----- 1 bandit4 bandit3   33 Apr 10 14:23 ...Hiding-From-You
bandit3@bandit:~/inhere$ cat ./...Hiding-From-You 
<password>
bandit3@bandit:~/inhere$ 


and we get the password to the next level.
