# Stacks and Queues
## Stack

A stack is a linear data structure that follows the Last-In-First-Out (LIFO) principle, meaning the last element added to the stack is the first one to be removed. Think of it as a stack of plates, where you can only add or remove plates from the top.

In JavaScript, you can implement a stack using an array or using a custom class. Let's start with the array-based implementation:

```javascript

// Creating an empty stack
let stack = [];

// Adding elements to the stack (push)
stack.push(10);
stack.push(20);
stack.push(30);

// Removing elements from the stack (pop)
let poppedElement = stack.pop(); // Removes and returns 30

console.log(poppedElement); // Output: 30
console.log(stack); // Output: [10, 20]
```
In the code above, we initialize an empty stack using an array. We can add elements to the stack using the push method, and remove elements from the stack using the pop method. The pop method removes the topmost element from the stack and returns it.

Class-based implementation example:

```javascript

class Stack {
  constructor() {
    this.stack = [];
  }

  push(element) {
    this.stack.push(element);
  }

  pop() {
    return this.stack.pop();
  }

  peek() {
    return this.stack[this.stack.length - 1];
  }

  isEmpty() {
    return this.stack.length === 0;
  }

  size() {
    return this.stack.length;
  }
}

// Usage:
let stack = new Stack();
stack.push(10);
stack.push(20);
stack.push(30);
console.log(stack.pop()); // Output: 30
console.log(stack.size()); // Output: 2
console.log(stack.peek()); // Output: 20
console.log(stack.isEmpty()); // Output: false
```
In this class-based implementation, we define the push and pop methods to add and remove elements from the stack, respectively. Additionally, we have a few other methods:

    peek returns the topmost element without removing it.
    isEmpty checks if the stack is empty.
    size returns the number of elements in the stack.

Now that we've covered stacks, let's move on to queues.

## Queue

A queue is a linear data structure that follows the First-In-First-Out (FIFO) principle, meaning the first element added to the queue is the first one to be removed. Think of it as a queue of people waiting in line, where the person who arrived first gets served first.

Similarly to stacks, you can implement a queue using an array or a custom class in JavaScript. Let's start with the array-based implementation:

```javascript

// Creating an empty queue
let queue = [];

// Adding elements to the queue (enqueue)
queue.push(10);
queue.push(20);
queue.push(30);

// Removing elements from the queue (dequeue)
let dequeuedElement = queue.shift(); // Removes and returns 10

console.log(dequeuedElement); // Output: 10
console.log(queue); // Output: [20, 30]
```
In the code above, we initialize an empty queue using an array. We can add elements to the queue using the push method, and remove elements from the queue using the shift method. The shift method removes the first element from the queue and returns it.

For a class-based implementation, here's an example:

```javascript

class Queue {
  constructor() {
    this.queue = [];
  }

  enqueue(element) {
    this.queue.push(element);
  }

  dequeue() {
    return this.queue.shift();
  }

  peek() {
    return this.queue[0];
  }

  isEmpty() {
    return this.queue.length === 0;
  }

  size() {
    return this.queue.length;
  }
}

// Usage:
let queue = new Queue();
queue.enqueue(10);
queue.enqueue(20);
queue.enqueue(30);
console.log(queue.dequeue()); // Output: 10
console.log(queue.size()); // Output: 2
console.log(queue.peek()); // Output: 20
console.log(queue.isEmpty()); // Output: false
```
In this class-based implementation, we define the enqueue and dequeue methods to add and remove elements from the queue, respectively. Additionally, we have the following methods:

    peek returns the first element in the queue without removing it.
    isEmpty checks if the queue is empty.
    size returns the number of elements in the queue.

That covers the basics of stacks and queues. I hope this explanation was helpful!!! 