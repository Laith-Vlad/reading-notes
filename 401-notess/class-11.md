##    What native Node.js module allows us to get started with Event Driven Programming?

To get started with Event Driven Programming in Node.js, you can use the built-in events module. This module provides an Event Emitter class that allows you to create and handle custom events in your Node.js applications. You can use the events module to define your own event-driven architecture and handle events asynchronously.

##    What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

Object-Oriented Programming (OOP) can bring several benefits when used in tandem with Event Driven Programming (EDP). By using OOP principles, you can create modular and reusable code by encapsulating related data and behavior into objects. This can make your code more organized, maintainable, and easier to understand.

When combined with EDP, OOP helps in modeling events as objects with their own properties and methods. Events can be represented as classes, and the behavior associated with those events can be encapsulated within the methods of those classes. This approach promotes code reusability and modularity, making it easier to manage and extend event-driven systems.

    Consider your knowledge of Event Driven Programming in the Web Browser, 
##    now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.

In the web browser, Event Driven Programming is commonly used to handle user interactions like button clicks, form submissions, or mouse movements. Similarly, on the backend using Node.js, Event Driven Programming allows us to handle events that occur in a server-side environment.

Let's imagine a scenario where you have a Node.js backend server that needs to handle multiple client requests simultaneously. Instead of processing each request sequentially, which could lead to delays and slow down the server, Node.js uses an event-driven architecture to handle these requests efficiently.

Node.js employs an event loop that continuously listens for events and triggers the associated event handlers. These events can include incoming HTTP requests, database queries completing, or file system operations finishing. When an event occurs, the associated event handler is invoked, allowing the server to respond promptly without blocking other requests.

This event-driven approach enables high scalability and performance in server applications. It allows Node.js to handle numerous concurrent connections efficiently, making it suitable for building real-time applications, chat systems, streaming services, and more.

## i want to learn about 
redux is very intresting subject to me packaging data and sending it upwards in react is very useful.