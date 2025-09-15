# Exp No: 36  
## Circular Queue 
---

### AIM  
To write a Python program with a function to insert float values into a Circular Queue.

---

### ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End

---

### PROGRAM

```
class Queue:
    def __init__(self,limit):
        self.queue=[]
        self.rear=0
        self.front=0
        self.limit=limit
    def isempty(self):
        if len(self.queue)==0:
            return True
        else:
            return False
    def enqueue(self,item):
        if len(self.queue)==self.limit:
            print("the queue is full")


        else:
            if self.front==self.limit:
                self.front=self.rear-1

            self.queue.insert(self.front,item)
            self.front+=1
    def dequeue(self):
        if len(self.queue)==0:
            print("the stack is under flow")
        else:
            if self.rear==self.limit:
                self.rear=0
            self.queue.pop(self.rear)
            self.rear+=1
    def display(self):
        print(self.queue)

size=int(input())
a=Queue(size)
str=input()
str1=input()
str2=input()

a.enqueue(str)
a.enqueue(str1)
a.enqueue(str2)
a.display()
a.dequeue()
a.display()


```

### OUTPUT
![image](https://github.com/user-attachments/assets/1183bf28-afc5-408c-8ae2-43540531efa7)


### RESULT
Thus, the Python program for inserting and deleting float values using a Circular Queue was successfully implemented using class and object concepts. The queue operations (enqueue, dequeue, and display) were tested and verified to work as expected.








