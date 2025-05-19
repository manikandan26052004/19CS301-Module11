# 19CS301-Module11
### EX: 11 a Singly Linked List (Traversal, Search and Delete)

### Aim: 
To write a Python function to traverse a linked list and display its elements in a specific format.


### Algorithm:

1.	Define a Node class with data and next attributes.
2.	Define a LinkedList class with methods to add nodes and traverse the list.
3.	In the traverse method, iterate through each node and collect the values.
4.	Print the list in the format: data1 -> data2 -> data3 -> None.



### Program:
```
#Reg.NO:212222220022
#Name:MANIKANDAN R
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None

class SLinkedList:
    def __init__(self):
        self.head = None

    def listprint(self):
        printval = self.head
        while printval is not None:
            print(printval.data)
            printval = printval.next

def main():
    my_list = SLinkedList()
    my_list.head = Node("Mon")
    e2 = Node("Tue")
    e3 = Node("Wed")
    my_list.head.next = e2
    e2.next = e3
    print("Linked List Contents:")
    my_list.listprint()

if __name__ == "__main__":
    main()
```
### Output:
![image](https://github.com/user-attachments/assets/959c411e-404a-4ed8-8bc4-6ef4a707ec80)


### Result: 
Thus, the given program is implemented and executed successfully .
 


