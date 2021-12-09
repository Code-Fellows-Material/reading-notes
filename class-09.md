# Class 09 Reading Notes

---

## Things I want to know more about

- How widely is functional programming used?

--- 

## Functional Programming Concepts

- [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

### Question Answers: 

*What is functional programming?*
-  "a programming paradigm...that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data"

*What is a pure function and how do we know if something is a pure function?*
- It is deterministic and has no observable side effects

*What are the benefits of a pure function?*
- Its very easy to test.

*What is immutability?*
- The ability to be unchanging. 


*What is Referential transparency?*
- If a function consistently yields the same result for the same input, it is said to be referentially transparent.

---

## Functional Programming Concepts

- [Node JS Tutorial for Beginners #6 - Modules and require](https://www.youtube.com/watch?v=xHLd36QoS4k)

### Question Answers: 

*What is a module?*
- A module is a JS file that holds a chunk of code and allows us to separate our our program.

*What does the word ‘require’ do?*
- Allows us to bring in modules to other files in our project.

*How do we bring another module into the file the we are working in?*
- We set a variable equal to the return value of the require('<module>') function, then we can use that variable. 

*What do we have to do to make a module available?*
- We have to export the functionality we want.