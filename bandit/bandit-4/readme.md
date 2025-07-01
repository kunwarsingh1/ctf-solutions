According to the bandit-4 page we have to login via ssh to get access to the shell of bandit-4 with username bandit4 and server bandit.labs.overthewire.org
on port 2220 with password from the previous level. After getting access to the shell we have to check the only human-readable file in the inhere directory.


So, we use the command ---
ssh bandit4@bandit.labs.overthewire.org -p 2220

after getting access to the shell we look into it using commands such as ----

bandit4@bandit:~/inhere$ find . -exec file {} \;
.: directory
./-file05: data
./-file03: data
./-file06: data
./-file02: data
./-file01: data
./-file09: data
./-file00: PGP Secret Sub-key -
./-file04: data
./-file08: data
./-file07: ASCII text
bandit4@bandit:~/inhere$ cat ./-file07
<password>
bandit4@bandit:~/inhere$ 
 


and we get the password to the next level.
