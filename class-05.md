# Class 05 Reading Notes

---

## Things I want to know more about

- How we can use higher order functions that return functions like the example from Eloquent JS.
- How higher order functions and composability tie together.
- Designing the application ahead of time.
- How to more cleanly structure my applications for better readability.


--- 

## React Docs - Thinking in React

- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

### Question Answers: 

- *What is the single responsibility principle and how does it apply to components?*
  - The single responsibility principle in this application means that a component should do one and only one thing, if it becomes more complex it should be split into small sub-components. 

- *What does it mean to build a ‘static’ version of your application?*
  - A 'static' version of your site would be one without any interactivity

- *Once you have a static application, what do you need to add?*
  - "...think of the minimal set of mutable state that your app needs." - TiR

- *What are the three questions you can ask to determine if something is state?*
  - 
                    Is it passed in from a parent via props? If so, it probably isn’t state.

                    Does it remain unchanged over time? If so, it probably isn’t state.

                    Can you compute it based on any other state or props in your component? If so, it isn’t state.

- *How can you identify where state needs to live?*
  
                    Identify every component that renders something based on that state.

                    Find a common owner component (a single component above all the components that need the state in the hierarchy).

                    Either the common owner or another component higher up in the hierarchy should own the state.

                    If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

                    Let’s run through this strategy for our application:


---

## Higher Order Functions

- [Higher Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

### Question Answers: 

- *What is a “higher-order function”?*
  - A function that operates on another function

- *Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?*
  - line 2 is returning an anonymous function that passes in the variable m and then compares whether that variable, m is greater than the variable n;
    - This one is a bit tricky to wrap your head around.

- *Explain how either map or reduce operates, with regards to higher-order functions.*
  - .map() takes as it's argument a function which it applies to each element within the array it was called on, returning a new array based on the return values of the passed in function. 