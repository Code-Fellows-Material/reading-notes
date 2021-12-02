# Class 03 Reading Notes

---

## Things I want to know more about

- Passing methods as references 
- When keys actually come in handy

--- 

## React Docs - lists and keys

- [React Docs - Forms](https://reactjs.org/docs/forms.html)

### Question Answers: 

- *What is a ‘Controlled Component’?*

    - An input form element whose value is controlled by React, the form also controls what happens in that form when the user submits data.

- *Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.*

    - We should update the state right away, because the displayed value will always be the state value.

- *How do we target what the user is entering if we have an event handler on an input field?*

    - We use the onChange method, utilizing the event object to access the target value, the target value being whatever the user has typed.

---

## The Spread Operator

- [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

### Question Answers: 

- *Why would we use a ternary operator?*

    - We would use a ternary operator to test some condition and run different code depending on the outcome of that test. 

- *Rewrite the following statement using a ternary statement*

                 x === y ? console.log(true) : console.log(false);

#### Side Notes: 

    - You can have nested ternary operators.
    - You can run multiple operations in a ternary, the operations must be comma seperated, and optionally can have paraenthesis around them.

                let isStudent = true;
                let price = 12;
                
                isStudent ? (
                    price = 8,
                    alert('Please check for student ID')
                ) : (
                    alert('Enjoy the movie')
                );