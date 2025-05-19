### 19CS301-Module11
### EX: 11.b Singly Linked List (Insertion and all operation)


### Aim: 
To write a Python program to add a new element at the start of a list.


### Algorithm:

1. Accept the number of elements and input the list.
2. Accept the new element to be added.
3. Use the insert(0, element) method to add the new element at the beginning of the list.
4. Display the updated list.

### Program:
```
#Reg.NO:212222220022
#Name:MANIKANDAN R
class Node:
  def __init__(self, data):
    self.data = data
    self.next = None

class LinkedList:
  def __init__(self):
    self.head = None

  def push_front(self, newElement):
    
    newNode=Node(newElement)
    newNode.next=self.head
    self.head=newNode

  def PrintList(self):
    temp = self.head
    if(temp != None):
      print("The list contains:", end=" ")
      while (temp != None):
        print(temp.data, end=" ")
        temp = temp.next
      print()
    else:
      print("The list is empty.")

MyList = LinkedList()

MyList.push_front(10)
MyList.push_front(20)
MyList.push_front(30)
MyList.PrintList()
```
### Output:
![image](https://github.com/user-attachments/assets/d2d6ba54-9808-4156-8e9b-f6ec925eecb2)

### Result: 
Thus, the given program is implemented and executed successfully .
 


