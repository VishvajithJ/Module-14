# Exp.No:38  
## Deque - DELETION

---

### AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  

---

### PROGRAM  

```

import collections
  
n1=input()
n2=input()
n3=input()

de = collections.deque([n1,n2,n3])



de.pop()


print ("The deque after deleting at right is : ")
print (de)
```

### OUTPUT
![image](https://github.com/user-attachments/assets/3dc3b198-3eef-491f-b891-dd4a598e0c02)


### RESULT
Thus, the Python program for deleting elements from the FRONT end of a deque using the built-in collections.deque class was written and executed. However, the code used pop() which removes from the right end (rear) instead of the front.
