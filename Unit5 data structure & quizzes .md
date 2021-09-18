## create a class Array

```py
class MyArray:
    #initialize
    def __init__ (self, size):
        self.size : int = size
        self.array: list = [None] * size
    #get the index of an item
    def get(self, index):
        print(f"The value with index {index} => {self.array[index]}")
    
    #insert an item
    def set(self, index, item):
        if index <= self.size:
            self.array[index] = item
            return print(f"updated array -> {self.array}")
        else:
            return print("Index out of range")

array_test = MyArray(7)

array_test.set(2,8)
array_test.set(0,4)
array_test.set(4,5)
array_test.set(5,2)
array_test.set(16,1)
array_test.get(1)

```
### testing

![Screen Shot 2021-09-18 at 12 43 27](https://user-images.githubusercontent.com/60457723/133871477-a7980be1-ed30-4684-af4a-38f0f95402e6.png)


## create a class queue

```py
class MyQueue:
    #initialize
    def __init__ (self):
        self.queue : list = []
    
    #enqueue -> add an item. first in.
    def enqueue(self, item):
        self.queue.append(item)
        print(f"current queue -> {self.queue}")
    
    #dequeue -> remove the item at first. first out.
    def dequeue(self):
        length = len(self.queue)
        if length == 0:
            print ("queue is empty")
        else:
            print(f"first queue -> {self.queue[0]}")
            del self.queue[0]
            print(f"updated queue -> {self.queue}")
            
    def is_empty(self):
        if self.queue:
            print("queue is not empty")
        else:
            print("queue is empty")

queue_test = MyQueue()
queue_test.enqueue(3)
queue_test.enqueue(5)
queue_test.enqueue(12)
queue_test.enqueue(15)
queue_test.dequeue()
queue_test.dequeue()
queue_test.enqueue(100)
queue_test.is_empty()
```
### testing

![Screen Shot 2021-09-18 at 12 19 47](https://user-images.githubusercontent.com/60457723/133870832-837dde3c-acb5-4b42-9a75-f4bd52c386d0.png)


## create a class stack

```py
class MyStack:
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
        print(f"last stack (the one will be removed first) -> {self.stack[-1]}")
        del self.stack[-1] 
        print(f"updated stack -> {self.stack}")
    
    #is_empty -> make sure if the list is empty 
    def is_empty(self):
        if self.stack:
            print ("stack is not empty now")
        else:
            print("stack is EMPTY")
        
stack_test = MyStack()
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

![Screen Shot 2021-09-18 at 12 21 14](https://user-images.githubusercontent.com/60457723/133870886-ce57710d-34cf-4568-a5b1-ca69487258de.png)


## Quiz 48
*inputs : a user enters ten integers*
*output : average of all inputs => HL students have to use queue method *

```.py
class MyQueue:
    def __init__ (self):
        self.queue : list = []
    
    def enqueue(self, item):
        self.queue.append(item)

    def dequeue(self):
        length = len(self.queue)
        if length == 0:
            print ("queue is empty")
        else:
            del self.queue[0]

class get_average(MyQueue):
    total = 0
    for i in range(10):
        user_input = int(input("please input a number: "))
        MyQueue.enqueue(user_input)
    for n in range(10):
        total += int(MyQueue.dequeue())
        average = total/10
        print(f"average => {average}")
 ```
 
 ### testing (incomplete)
 ![Screen Shot 2021-09-18 at 13 04 35](https://user-images.githubusercontent.com/60457723/133871921-2e261001-8e90-4459-a541-f926f9d6a102.png)


## Quiz 49
*Inputs:10 Ib scores(1-7) from the user*
*Output: average of the scores*

```.py

```

### testing 
