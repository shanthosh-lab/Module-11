## 🔍 Singly Linked List-To Search an Element in a Linked List
This project contains a simple implementation of a singly linked list in Python, allowing insertion and searching of elements.

## 🎯 Aim
To write a Python program to search for a given element in a singly linked list using object-oriented programming principles.

## 🧠 Algorithm
1. Define a Node class with data and next attributes.
2. Define a LinkedList class with:
3. A head pointer initialized to None.
4. A push() method to add elements at the beginning.
5. A search() method to check whether a given value exists.
6. Create a LinkedList instance.
7. Insert the elements 10, 30, 11, 21, 14 using push() (which results in reverse order).
8. Read an integer input from the user.
9. Use search() to check if the element exists in the list.
10. Output "Yes" if found, else "No".
## 💻 Program
class Node:

def init(self, data):

self.data = data

self.next = None
class LinkedList:

def init(self):

self.head = None
def push(self, new_data):

new_node = Node(new_data)

new_node.next = self.head

self.head = new_node
def search(self, x):

current = self.head

while current != None:
    
    if current.data == x:

        return True
    
    current = current.next

return False
llist = LinkedList()

llist.push(10);

llist.push(30);

llist.push(11);

llist.push(21);

llist.push(14);

data = int(input())

if llist.search(data):

print("Yes") else:

print("No")

## Sample Output

<img width="320" height="177" alt="491474505-d197da23-0258-450a-99d7-bee9be73dacf" src="https://github.com/user-attachments/assets/d8917c0f-2943-4e11-8d78-dacec3dea7a8" />
## Result

The program is excuted and verified.
