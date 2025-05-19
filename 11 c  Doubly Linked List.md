### EX: 11.C Doubly Linked List (Traversal, Search and Delete)

### Aim:
To write a Python program to traverse and display the elements in a doubly linked list.
### Algorithm:
1. Define a Node class with data, prev, and next pointers.
2. Define a DoublyLinkedList class to manage nodes.
3. Implement a method to append nodes at the end.
4. Implement a method to traverse the list from the head to the end.
5. Display each element during traversal.

### Program:
```
#Reg.NO:212222220022
#Name:MANIKANDAN R
class Node:
    def __init__(self, data):
        self.item = data
        self.nref = None
        self.pref = None

class DoublyLinkedList:
    def __init__(self):
        self.start_node = None

    def insert_in_emptylist(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
        else:
            print("list is not empty")
            
    def insert_at_start(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
            print("node inserted")
            return
        new_node = Node(data)
        new_node.nref = self.start_node
        self.start_node.pref = new_node
        self.start_node = new_node
        
    def insert_at_end(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
            return
        n = self.start_node
        while n.nref is not None:
            n = n.nref
        new_node = Node(data)
        n.nref = new_node
        new_node.pref = n
        
    def traverse_list(self):
        if self.start_node is None:
            print("List has no element")
            return 
        else:
            n=self.start_node
            while n is not None:
                print(n.item," ")
                n=n.nref
                
new_linked_list = DoublyLinkedList()
new_linked_list.insert_in_emptylist(50)
new_linked_list.insert_at_start(10)
new_linked_list.insert_at_start(5)
new_linked_list.insert_at_start(18)
new_linked_list.insert_at_end(29)
new_linked_list.insert_at_end(39)
new_linked_list.insert_at_end(49)
new_linked_list.traverse_list()
        

```
### Output:
![image](https://github.com/user-attachments/assets/cf4cf7eb-f229-4f49-9c52-c64b7fcc4a5a)

### Result: 
Thus, the given program is implemented and executed successfully.
 


