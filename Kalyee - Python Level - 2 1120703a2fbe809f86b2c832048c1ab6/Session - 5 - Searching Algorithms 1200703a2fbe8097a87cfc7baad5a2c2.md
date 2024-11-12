# Session - 5 - Searching Algorithms

### Linear Search Algorithm

![image.png](Session%20-%205%20-%20Searching%20Algorithms%201200703a2fbe8097a87cfc7baad5a2c2/image.png)

```python

lst = [4,2,4,5,4,3,2,4,6,77,53]

element = 63 

present = False 

for i in range(len(lst)) : 
    if lst[i] == element : 
        present = True 
        break 

if present == False : 
    print("Element do not exist in the given list ")

else : 
    print("Element is present at position " , i )

```

### Binary Search Algorithm

![image.png](Session%20-%205%20-%20Searching%20Algorithms%201200703a2fbe8097a87cfc7baad5a2c2/image%201.png)

```python

lst = [2,3,4,6,7,8,9,12,34,67,76,78,97]

element = 67 

low = 0 
high = len(lst) - 1 

while low <= high : 
    mid = (low+high)//2 

    if ( lst[mid] == element ) : 
        print("Element " , element , "is present at location : " , mid) 
        break

    elif ( element > lst[mid] ) : 
        low = mid + 1 

    else : 
        high = mid - 1 

```