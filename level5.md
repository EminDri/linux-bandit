# Level 5

### Goal: The password for the next level is stored in the only human-readable file in the inhere directory.

## Solution: 
1. I used ```cd inhere``` to enter inhere directory.
2. Once inside inhere directory I used ```ls``` to view files.
3. After that I used ```file ./*``` to view what type of file each file is and I identified file ```-file07``` as the text file.
4. I then used ```cat ./-file07``` as it starts with a - so it needs to escape it first.
5. Then I used this password to log into bandit6 user using ```ssh``` command.

## Thought Process:
- As there was multiple files and I needed to know which one was a text file I used the ```file``` command followed by ```*``` as all of the files had to be checked.
- Also thought to use ```./``` as the file name started with ```-```.
