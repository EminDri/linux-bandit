# Level 6

### Goal: The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable<b>
1033 bytes in size<b>
not executable<b>

## Solution: 
1. Firstly, I entered the ```inhere``` directory using ```cd inhere```.
2. Secondly, I used the ```find -type f -size 1033c``` command to search for a file inside of inhere with file size 1033.
3. Lastly, I used ```cat ./maybehere07/.file2``` to view the lines of text in the ```.file2``` file.

## Thought Process:
- I knew that the find command without filtering wasn't enough to find the specific file, so I used filters such as ```-type``` and ```-size```.
