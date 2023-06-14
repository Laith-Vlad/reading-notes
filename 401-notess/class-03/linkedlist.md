# Linked lists
## code demostrations for linked lists
```javascript
// Node class representing a node in the linked list
class Node {
  constructor(data) {
    this.data = data; // Value stored in the node
    this.next = null; // Reference to the next node
  }
}

// Linked list class
class LinkedList {
  constructor() {
    this.head = null; // First node in the list
  }

  // Method to add a new element at the end of the linked list
  add(data) {
    const newNode = new Node(data); // Create a new node with the given data

    if (this.head === null) {
      this.head = newNode; // If the list is empty, set the new node as the head
    } else {
      let current = this.head;
      while (current.next !== null) {
        current = current.next; // Traverse to the last node
      }
      current.next = newNode; // Update the last node's next reference
    }
  }

  // Method to remove the first occurrence of a given element from the linked list
  remove(data) {
    if (this.head === null) {
      return; // If the list is empty, nothing to remove
    }

    if (this.head.data === data) {
      this.head = this.head.next; // If the head node contains the data, update the head
      return;
    }

    let current = this.head;
    let prev = null;

    while (current !== null) {
      if (current.data === data) {
        prev.next = current.next; // Adjust references to skip over the node
        return;
      }
      prev = current;
      current = current.next;
    }
  }
}

// Example usage
const linkedList = new LinkedList();
linkedList.add(5);
linkedList.add(10);
linkedList.add(15);
linkedList.remove(10);

console.log(linkedList);
```
**Linked List:**

A linked list is a linear data structure where elements are stored in separate objects called nodes. Each node contains the data value and a reference (or link) to the next node in the sequence. The first node is called the head, and the last node points to null, indicating the end of the list.

Linked lists offer dynamic memory allocation, efficient element insertion and deletion, and flexible size. However, accessing elements by index is slower compared to arrays because linked lists require traversing from the head to the desired node.

**Singly Linked List:**

In a singly linked list, each node contains a reference to the next node. Traversing the list can only be done in one direction (forward). Inserting or removing a node in the middle of the list requires updating the references of the adjacent nodes.

**Doubly Linked List:**

A doubly linked list extends the singly linked list by including an additional reference to the previous node in each node. This allows traversing the list in both directions (forward and backward). Insertion or removal of a node becomes more efficient as it requires updating the references of both adjacent nodes.

**Big O Complexity of Linked List:**

- Accessing an element by index: O(n) - In worst case, you may need to traverse the entire list to reach the desired index.
- Insertion or deletion at the beginning: O(1) - Updating the head reference only requires a few operations.
- Insertion or deletion at the end: O(n) - You need to traverse the list to reach the last node.
- Insertion or deletion in the middle: O(n) - Requires traversing the list to find the desired position.

Keep in mind that these complexities may vary based on the specific implementation and operations performed on the linked list.