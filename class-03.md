# Class 03 Reading Notes

---

## Things I want to know more about

- Passing methods as references 
- When keys actually come in handy

--- 

## React Docs - lists and keys

- [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

### Question Answers: 

- What does .map() return?
    - A new, modified array.

- If I want to loop through an array and display each value in JSX, how do I do that in React?
    - using the map() method, you can surround each value in curly braces and a component tag or your chosing, then return that. The map method will output a new array with these inside, and react can render an array of components. 

- Each list item needs a unique "key".
    - *A “key” is a special string attribute you need to include when creating lists of elements.* -ReactDocs
    - **key is a STRING**
    - **Best to use the id froom your data:** `<li key={todo.id}>{todo.text}</li>` **You can use the index value of the array as a last resort**  -ReactDocs

- What is the purpose of a key?
    - *Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.* -ReactDocs


#### Side Notes:

-*Keys Must Only Be Unique Among Siblings. We can use the same keys when we produce two different arrays.* -ReactDocs

---

## The Spread Operator

- [How to Use the Spread Operator \(…) in JavaScript, by Dr. Derek Austin](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

### Question Answers: 

- What is the spread operator?
    - *The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.* -Dr. D.A.
    - The spread operator splits an array into it's individual components.

- List 4 things that the spread operator can do.
    - Copying an array
    - Concatenating or combining arrays
    - Using an array as arguments
    - Adding to state in React

- Give an example of using the spread operator to combine two arrays.

                let someArr = [1, 2];
                let diffArr = [3, 4, 5];

                let combArr = [...someArr, ...diffArr];

                console.log(combArr); // [1, 2, 3, 4, 5];

- Give an example of using the spread operator to add a new item to an array.


                let diffArr = [3, 4, 5];

                let combArr = [1, 2, ...diffArr];

                console.log(combArr); // [1, 2, 3, 4, 5];

- Give an example of using the spread operator to combine two objects into one.

                let someObj = {first: "Kellen"};
                let diffObj = {last: "Linse"};

                let fullName = {...someObj, ...diffObj};

                console.log(fullName); // {first: "Kellen", last: "Linse"};

---

## How to Pass Functions Between Components

- [React - How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

### Question Answers: 

- In the video, what is the first step that the developer does to pass functions between components?

    - He defines the function he wishes to pass.

- In your own words, what does the increment function do?

    - It updates the count property of an indivdual opbject in the people array.

- How can you pass a method from a parent component into a child component?

    - You can pass a reference to the function through props, just like you would a variable. 

- How does the child component invoke a method that was passed to it from a parent component?

    - In a method defined within it's own class (could propbably use an anonymous function in something like a clickHandler too).
