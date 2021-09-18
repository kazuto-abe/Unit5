## create a class "Array"*

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
## create a class of queue

```py

```

## create a class of stack

```py
class Stack:
    # initialize
    def __init__(self):
        self.stack: list = []
    
    #push -> add items to the list. (first in)
    def push(self, item):
        self.stack.append(item)
        print(f"new item -> {item}")
        print(f"Current stack -> {self.stack}")
    
    #pop -> pull an item added at LAST. (last out)
    def pop(self):
        print(f"Front row (the one will be removed first) -> {self.stack[-1]}")
        del self.stack[-1] 
        print(f"updated stack -> {self.stack}")
    
    #is_empty -> make sure if the list is empty 
    def is_empty(self):
        if self.stack:
            print ("stack is not empty now")
        else:
            print("stack is EMPTY")
        
stack_test = Stack()
stack_test.push(1)
stack_test.push(3)
stack_test.push(5)
stack_test.push(7)
stack_test.pop()
stack_test.pop()
stack_test.push(25)
stack_test.is_empty()
```

### testing

![Screen Shot 2021-09-18 at 11 55 20](https://user-images.githubusercontent.com/60457723/133870146-73520cbd-eb5a-4318-b5ac-0fa5234ec9cd.png)


## Quiz 47

2D array , chessboard 

## Quiz 48
get average using queue 


## Quiz 49
store IB score using stack 

