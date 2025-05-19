# EX 6D BRUTE FORCE ALGORITHM
## DATE: 17/05/2025
## AIM:
To write a python program using brute force method of searching for the given substring in the main string.

## Algorithm
1.Start from index 0 in the main string and try to match the substring at every position.

2.Compare characters one by one from the current position in the main string to the substring.

3.If all characters match, return the current index as the starting point of the match.

4.If a mismatch is found, move to the next index in the main string and repeat.

5.If no match is found after checking all valid positions, return -1.
## Program:

To implement the program using brute force method of searching for the given substring in the main string.

Developed by: Vidhyasri k

Register Number:212222230170

```PYTHON
import re
def match(string,sub):
    pattern = re.compile(str2)
    r = pattern.search(str1)
    while r:
        print("Found at index {}".format(r.start()))
        r = pattern.search(str1,r.start()+1)    

str1=input()
str2=input()
```

## Output:
![image](https://github.com/user-attachments/assets/e91763b2-05e6-4a7f-bf7e-b72dbf723a4c)

## Result:
Thus the above program was executed successfully for searching the substring at respective index.
