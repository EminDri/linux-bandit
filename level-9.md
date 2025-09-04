# Level 9

### Goal: The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Solution: 
1. Firstly, used the command ```sort data.txt | uniq -c``` to sort the text in order then count duplicates.
2. The password was the one which had a 1 next to it to show that it had no duplicate, I then used it to log into user bandit9 using ```ssh```.
   
## Thought Process:
- I tried to use ```uniq -c``` on it's own but it didn't work, but I then found out that the ```uniq``` command only finds duplicates that are consecutive, so I used the sort command to make sure they are in order and appear consecutively.
