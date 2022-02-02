# 401 - Class 06 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. Explain what a “Singleton” is (in Computer Science terms):
     - "In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system." -wikipedia

2. Explain how the Singleton pattern can be used with Node modules, specifically with classes:
     - The singleton pattern is of use when you need to track the state of an object across different files and functions. If the object is modified in one place, you want those changes to be present in other places. It allows for a type of global object state. 


3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
      - The singleton pattern seems to make the most sense, but it would vary by application I suppose.


RESOURCES: [JavaScript Design Patterns: The Singleton](https://www.sitepoint.com/javascript-design-patterns-singleton/)

--- 

## Vocabulary Terms

- Router Middleware: 
  - Router Middleware is middleware that happens server side that runs once the server has received a request, but before the server sends it's response.
  - [Writing Express Middleware](https://expressjs.com/en/guide/writing-middleware.html)

- Dynamic Module Loading:
  - Dynamic Module Loading uses the import() expression."The import(module) expression loads the module and returns a promise that resolves into a module object that contains all its exports. It can be called from any place in the code."

  ```js
  let modulePath = prompt("Which module to load?");

  import(modulePath)
    .then(obj => <module object>)
    .catch(err => <loading error, e.g. if no such module>)
  ``` 
  - [Dynamic imports](https://javascript.info/modules-dynamic-imports)

- Singleton Pattern: 
  - "In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system." -wikipedia

- CRUD -> REST Method Matches:

  - Create = POST
  - Read = GET
  - Update = PUT, PATCH
  - Delete = DELETE

- Mock Testing: 
  - "Mock functions allow you to test the links between code by erasing the actual implementation of a function, capturing calls to the function (and the parameters passed in those calls, capturing instances of constructor functions when instantiated with new, and allowing test-time configuration of return values"
  - [Mock Functions in Jest](https://jestjs.io/docs/mock-functions)

--- 

## Preview 

Which 3 things had you heard about previously and now have better clarity on?
   - Singletons. It makes sense when you think of it as retaining global object state, which it much easier in different languages.

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - Authentication, encryption, how user passwords are stored.

What are you most excited about trying to implement or see how it works?
   - Encryption.