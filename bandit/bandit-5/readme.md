According to the bandit-5 page we have to login via ssh to get access to the shell of bandit-5 with username bandit5 and server bandit.labs.overthewire.org
on port 2220 with password from the previous level. After getting access to the shell we have to check the only human-readable file in the inhere directory.


So, we use the command ---
ssh bandit5@bandit.labs.overthewire.org -p 2220

after getting access to the shell we look into it using commands such as ----


bandit5@bandit:~/inhere$ find . -type f ! -executable -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cd maybehere07
bandit5@bandit:~/inhere/maybehere07$ ls
-file1  -file2  -file3  spaces file1  spaces file2  spaces file3
bandit5@bandit:~/inhere/maybehere07$ cat ./.file2
<password>
