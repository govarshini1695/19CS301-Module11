SINGLY LINKED LIST-DELETE THE FIRST ELEMENT

AIM: 
To write the python program to delete the first element in the given linked list.

ALGORITHM:

STEP 1:Start the program.
STEP 2:Check if the linked list is empty. If it is, return without deleting anything.
STEP 3:Update the head pointer to point to the second node.
STEP 4:Delete the original head node to free memory (optional in Python, handled by garbage collection).
STEP 5:delete_first() checks if the list is empty before proceeding.
STEP 6:If not empty, it moves the head pointer to the next node, effectively removing the first element.
STEP 7:The display() function prints the list before and after deletion.

PROGRAM:

```
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        
class delete_front:
    def __init__(self):
        self.head = None
  
    def removeFirstNode(self):
        if not self.head:
            return None
        temp=self.head
        self.head=self.head.next
        temp=None
        
    def push(self, data):
        if self.head is None:
            self.head = Node(data)
            return
        temp = Node(data)
        temp.next = self.head
        self.head = temp
        
    def display(self):
        temp1 = self.head
        while temp1 is not None:
            print(temp1.data , end =" ")
            temp1 = temp1.next
  

dfront = delete_front()
val = int(input("Enter the number of elements to push:\n"))
for i in range(val):
    data = int(input())
    dfront.push(data)

dfront.removeFirstNode()
      
dfront.display()
```

OUTPUT:

![image](https://github.com/user-attachments/assets/7a839f0e-3316-4726-a379-a21df71c4b18)


RESULT:

Thus the program to delete the first element in the given linked list is executed successfully.

