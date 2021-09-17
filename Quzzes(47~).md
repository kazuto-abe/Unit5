## Quiz 47

## Quiz 48

## Quiz 49

## Homework for sep12
*create a class "Array"*

```py
class Array:
    def __init__ (self, size, data):
        self.size = size
        self.data = data
    
    def get(self, index):
        if index <=  self.size:
            print (self.data[index])
        else:
            print ("index out of range")
    
    def set(self, index, value):
        if index <= self.size:
            print(self.data[index]) = value
        print(self.data)
        else:
            print ("index out of range")

Array_1 = Array([1,3,5,10,0])

Array_1.get(1)
```
```py
class Stack:
    def __init__(self):
        self.stack = []
    def push(self, item):
        self.stack.append(item)
    def pop(self):
        result = self.stack[-1] 
        del self.stack[-1]  
        return result

```


