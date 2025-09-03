# Level 3

### Goal: The password for the next level is stored in a file called 'spaces in this filename' located in the home directory

## Solution: 
1. Use ```cat "spaces in this file name"``` to view the line of text in this file.
2. Then use this password when doing the ssh login.

## Thought Process:
- If I use ```cat spaces in the filename``` it will take each word as a separate argument due to the spaces, so I used quotation marks.
