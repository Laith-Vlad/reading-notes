# Express REST API
## ES 6 review

- Classes are a template for creating objects.
- No, class declarations cannot be hoisted in most programming languages.
- A constructor is a special method within a class that is automatically called when an object is created. "This" refers to the current instance of the class and allows access to its properties and methods.
## Using Express Routing
- In Express, routing refers to handling HTTP requests at specific URLs or paths.

- The route path determines the URL pattern to match, while the route method specifies the HTTP method to match.

- next is added as a parameter to a route handler or middleware to pass control to the next middleware or route handler in the chain. If next is passed to your middleware, you must call it to ensure the application continues to the next middleware or route handler.
 ## Express Routing
- An Express Router is a module in Express.js that helps organize and handle routes for HTTP requests.

- express.Router() is initialized by requiring the Express module and invoking the Router() method.
- Route middleware in Express is used to perform actions on requests or responses before they are handled by route handlers, such as authentication, logging, validation, error handling