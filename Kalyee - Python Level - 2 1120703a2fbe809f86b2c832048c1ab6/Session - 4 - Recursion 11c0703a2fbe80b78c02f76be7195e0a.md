# Session - 4 - Recursion

```python

def greet(n) : 

    # base case 
    if n < 1 : 
        return 

    print("Hello how are you ? ")

    n = n - 1

    greet(n) 

greet(5)
```

### Finding Factorial of a number using Recursion

```python
def factorial(n) : 

    # base case 
    if n < 1 :
        return 1 

    return n * factorial(n-1)

print(factorial(4))
```

### Fibonaccie Sequence

```python

first = 0
second = 1 

terms = int(input("Enter number of terms for fibb series : "))

for i in range(terms):

    current = first + second 

    print(current)

    first = second 
    second = current 
```

### Extra

```json
Session - 4 - Recursion 

def greet(n) : 

    # base case 
    if n < 1 : 
        return 

    print("Hello how are you ? ")

    n = n - 1

    greet(n) 

greet(5)

Finding Factorial of a number using Recursion
def factorial(n) : 

    # base case 
    if n < 1 :
        return 1 

    return n * factorial(n-1)

print(factorial(4))

```