# EX 6B KNAPSACK PROBLEM
## DATE: 03/05/25
## AIM:
To demonstrate a python program using dynamic programming for 0/1 knapsack problem.

## Algorithm

1. Base Case: If n == 0 or W == 0, return 0.

2. If item too heavy: If wt[n-1] > W, skip it:
   → return knapSack(W, wt, val, n-1)

3. Else: Take max of:

   Include item: val[n-1] + knapSack(W - wt[n-1], wt, val, n-1)

4. Exclude item: knapSack(W, wt, val, n-1)

5. Return the maximum of the above two choices.

## Program:

To implement the program for 0/1 knapsack problem.

Developed by: Vidhyasri k

Register Number: 212222230170


```
def knapSack(W, wt, val, n):

     if n==0 or W==0:
         return 0
     if wt[n-1]>W:
         return knapSack(W, wt, val, n-1)
     return max(val[n-1]+knapSack(W-wt[n-1], wt, val, n-1),knapSack(W, wt, val, n-1))

x=int(input())
y=int(input())
W=int(input())
val=[]
wt=[]
for i in range(x):
    val.append(int(input()))
for y in range(y):
    wt.append(int(input()))
n = len(val)
print('The maximum value that can be put in a knapsack of capacity W is: ',knapSack(W, wt, val, n))
```

## Output:
![image](https://github.com/user-attachments/assets/ff4b94e5-885b-4b71-97d7-f52db4f5c580)


## Result:
Thus the program was executed successfully for finding the maximum value that can be put in a knap sack of capacity .
