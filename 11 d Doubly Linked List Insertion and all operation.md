### EX: 11.d Doubly Linked List (Insertion and all operation)


### Aim:
To write a Python function to insert elements at the beginning of a doubly linked list.

### Algorithm:
1.	Define a Node class with data, prev, and next pointers.
2.	Define a DoublyLinkedList class.
3.	Implement an insert_at_beginning(data) method:
         -	Create a new node.
         -	Set its next to the current head.
         -	Update the current head’s prev to the new node (if head exists).
         -	Update head to the new node.
4.	Implement a method to display the list.


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
        new_node.nref=self.start_node
        self.start_node.pref = new_node
        self.start_node = new_node
        
        
    def traverse_list(self):
        if self.start_node is None:
            print("List has no element")
            return
        else:
            n = self.start_node
            while n is not None:
                print(n.item , " ")
                n = n.nref
                
new_linked_list = DoublyLinkedList()
new_linked_list.insert_in_emptylist(40)
new_linked_list.insert_at_start(30)
new_linked_list.insert_at_start(20)
new_linked_list.insert_at_start(10)
new_linked_list.traverse_list()
```
### Output:
 
![image](https://github.com/user-attachments/assets/ee72eaf2-3023-49a9-8de5-1a6369f17e68)

 

### Result: 
Thus, the given program is implemented and executed successfully.
