# Level 1

### Goal: The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Solution: 
1. In home directory I used ```bash ls``` to see the files in the directory.
2. Then I used ```bash cat readme``` to view the contents of the readme file.
3. I then copied the password which was in the readme file and used this file when logging into bandit1 user using ```bash ssh -p 2220 bandit1@bandit.labs.overwire.org```.
