# Level 7

### Goal: The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

## Solution: 
1. Firstly, I used ```ls -a``` to make sure every file and directory is viewed.
2. I then used ```cd ..``` to go into the home directory.
3. After that I used ```ls -a``` once again to see all the directories and files.
4. Then I used ```find / -type f -user bandit7 -group bandit6 -size 33c``` to find the files which have these properties by checking everywhere.
5. In the list I found the file ```bandit7.password``` which had these properties and used ```cat /var/lib/dpkg/info/bandit7.password``` to view the lines of text.
6. Lastly, I use the password to log into bandit7 user using ```ssh``` command.
   
## Thought Process:
- I made sure to filter for the needed properties.
- Realised that I had to move into the ```home``` directory to find the needed directory and files.
- Also realised that using the command ```find / -type f -user bandit7 -group bandit6 -size 33c``` it views all the permission denied messages so I could've used ```2>/dev/null``` to get rid of the permission denied messages.
