# 401 - Class 03 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. Name 3 real world use cases where you’d want to change the request with custom middleware
   - Authentication
   - Logger
   - Security

2. True or false: The route handler is middleware?
   - Depends on how it is implemented I think.

3. In what ways can a middleware function end the process and send data to the browser?
   - By not calling next and calling res.send instead.

4. At what point in the request lifecycle can you “inject” middleware?
   - After the request is received, before the router.

5. What can cause express to error with “Request headers sent twice, cannot start a second response”
   - calling res.send after you've already called res.send


## Vocabulary Terms

Middleware: Express definition: 

>Middleware functions can perform the following tasks:
>
> - Execute any code.
> - Make changes to the request and the response objects.
> - End the request-response cycle.
> - Call the next middleware function in the stack.

Request Object: Express Definition:

> The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on. In this documentation and by convention, the object is always referred to as req (and the HTTP response is res) but its actual name is determined by the parameters to the callback function in which you’re working.

Response Object:

> The res object represents the HTTP response that an Express app sends when it gets an HTTP request.

Application Middleware:

> Application middleware is middleware we write or a library has written that goes before the route handler. Can use the app.use method to inject application middleware.

Routing Middleware:

> Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().

Test Driven Development:

> Test Driven Development is a style of programming where tests are written first, then code is written that will pass those tests after.
Jest: A node package, testing suite, that assists with code testing and test driven development.

Behavioral Testing:

> Tests in Behavior driven testing are most often focused on the behavior of users rather than the technical functions of the software. - [Source](https://www.katalon.com/sa/behavior-driven-testing/)