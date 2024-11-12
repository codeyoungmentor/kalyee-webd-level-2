# Session - 6 - Sorting Algorithm

![image.png](Session%20-%206%20-%20Sorting%20Algorithm%2012e0703a2fbe802cb028f303fec4ff05/image.png)

```python

lst = [8,6,9,7,5,14,32,3,78,65]

smallest_index = 0 

for i in range(0 , len(lst)):

    if lst[i] < lst[smallest_index] : 
        smallest_index = i 

print(lst[smallest_index])
```

[https://www.notion.so](https://www.notion.so)

![image.png](Session%20-%206%20-%20Sorting%20Algorithm%2012e0703a2fbe802cb028f303fec4ff05/image%201.png)

```json
# bubble sort algorithm

lst = [45,3,24,99,23,1,56,54]

for j in range(len(lst)-1):
    for i in range(len(lst)-1):
        if lst[i] > lst[i+1] : 
            #swap
            lst[i] , lst[i+1] = lst[i+1] , lst[i]

print(lst)

```

![image.png](Session%20-%206%20-%20Sorting%20Algorithm%2012e0703a2fbe802cb028f303fec4ff05/image%202.png)