## 📚 Singly Linked List : Find the Middle Node of a Singly Linked List

This Python program demonstrates how to create a singly linked list and print the data of the third node in the list. The program builds the list by inserting elements at the beginning and then traverses it to reach the third node.

## 🎯 Aim
To write a Python program that: -Creates a singly linked list. -Traverses the list to find and display the data of the third node (if it exists).

## 🧠 Algorithm
1. Node Class: Define a Node class to represent each node in the singly linked list. Each node has two attributes: data and next..
2. LinkedList Class: Define a LinkedList class that manages the linked list with methods to: -'push(new_data)': Insert a new node at the beginning of the list. -'printMiddle()': Traverse the list using a counter and print the data of the third node.
3. Input: The program reads 5 integers from the user and inserts them one by one at the head of the linked list.
4. Middle Finding: Start from the head and move to the next node while maintaining a counter. When the counter reaches 3, print the current node’s data.
5. Output: Displays the data value of the third node in the linked list

## 💻 Program 

class Node: def init(self, value): self.data = value self.next = None
class LinkedList:

def init(self):

self.head = None
def push(self, new_data):

new_node = Node(new_data)
new_node.next = self.head
self.head = new_node
def printMiddle(self):

temp = self.head
count = 1
while temp is not None:
    if count==3:
        print(temp.data)
    temp = temp.next
    count+=1
llist = LinkedList() for i in range(5): value = int(input()) llist.push(value)

llist.printMiddle()

## Sample Input & Output
<img width="379" height="213" alt="491471577-3b591c0d-8514-4150-812b-d970a0c3b7c0" src="https://github.com/user-attachments/assets/76d4b3c6-689d-4832-984c-1ebceab9cc72" />

## Result
The program is excuted and verified.
