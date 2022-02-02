# 401 - Class 12 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. What is the benefit of transforming data into packets?
  - It optimizes the use of the channel capacity available in digital networks, and minimizes the time it takes for data to pass across the network.

2. UDP is often refereed to as a connectionless protocol. Why is this?
  - Because a connection route is not pre-defined, it includes multiple packets, each individually routed.
   
4. Can a socket server application have multiple socket connections?
  - Yes, on different ports.

5. Can a socket connection application be connected to multiple socket servers?
  - You can only have one connection per socket, but you can have multiple sockets for connecting more than one server.

6. Can an application be both a socket server and a socket connection?
  - Yes, and echo server is an example of this. 

--- 

## Vocabulary Terms

  - Observer Pattern:"Observer pattern is used when there is one-to-many relationship between objects such as if one object is modified, its depenedent objects are to be notified automatically. Observer pattern falls under behavioral pattern category."

  [Resource](https://www.tutorialspoint.com/design_pattern/observer_pattern.htm)

 - Listener: Event listeners registered for an event type may either be JavaScript functions or objects with a handleEvent property whose value is a function.
  
  [Resource](https://nodejs.org/api/events.html#event-listener)

 - Event Handler: An event handler is a function or set of instructions that runs for a given listener once that listener has received the event it was listening for. 

 - Event Driven Programming: "Event-driven programming depends upon an event loop that is always listening for the new incoming events. The working of event-driven programming is dependent upon events. Once an event loops, then events decide what to execute and in what order."

  ![Resource]('./../driven.jpg')
 
  [Resource](https://nodejs.org/api/events.html#event-listener)

 - Event Loop: The event loop is a constantly running process that monitors both the callback queue and the call stack. 

 - Event Queue: A First in First out list of the next events to have the event loop trigger.

 - Call Stack: A Last in First out list of the currently running functions within the event loop.

 - Emit/Raise/Trigger: A listener listens for a singular predefined event to be emitted somewhere else, either in the same code base or externally, then once that event has happened, it triggers the listeners callback function to run.

 - Subscribe: In this context, subscribe refers to a listener begin set up to listen for a certain event to take place from a specific place. It can be said to be subscribing to listen for that event. 

 - database: A database is an organized collection of structured information, or data, typically stored electronically in a computer system. 
--- 

