# Level 4

### Goal: The password for the next level is stored in a hidden file in the inhere directory.

## Solution: 
1. Use ```ls``` to check which directories and files exist.
2. Use ```cd inhere``` to enter inhere directory.
3. Once inside inhere directory use ```ls -a``` to view all files.
4. Finally use ```cat ...Hiding-From-You``` to display the lines of text in this file to reveal the password.

## Thought Process:
- Once inside the inhere directory I must use ```ls -a``` to view ALL files instead of using ```ls``` on it's own, which would<b>
only view non-hidden files. But as the hidden file's name starts with . it will be hidden so can't be viewed with ```ls```.
