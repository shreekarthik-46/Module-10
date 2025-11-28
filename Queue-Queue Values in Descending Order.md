# 10)a) Queue-Queue Values in Descending Order Using Python 

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

##  Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

##  Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

##  Program: 
```
from queue import PriorityQueue
que=PriorityQueue()
n=int(input())
l=[]
for i in range(n):
    l.append(int(input()))
for number in l:
    que.put((-number, number))
while not que.empty():
    print(que.get()[1])
```

### Output:

![queue-des](https://github.com/user-attachments/assets/43542bc8-7ad5-44e8-9d39-3f08848fdc19)

## Result:
Thua a Python program to:
Accept user inputs into a list (queue)
Remove the first two elements (simulating dequeue)
Display the remaining values in **descending order** is created.

