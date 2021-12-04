# Class 03 Reading Notes

---

## Things I want to know more about

- What other types of architecture are there?
- What other programs use a component based architecture?

--- 

## Component-Based Architecture

- [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

### Question Answers: 

- *What is a “component”?*
        "A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface."

    - Can be thought of like a building block that can be moved around an re-used. 

- *What are the charactistics of a component?*

                    Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

                    Replaceable − Components may be freely substituted with other similar components.

                    Not context specific − Components are designed to operate in different environments and contexts.

                    Extensible − A component can be extended from existing components to provide new behavior.

                    Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

                    Independent − Components are designed to have minimal dependencies on other components.

- *What are the advantages of using component-based architecture?*

    - Reusability, Ease of Deployment, and Ease of Deployement are three adcantages of using component based architecture.


## What is “Props” and how to use it in React?

- [What is “Props” and how to use it in React?](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

- This story is behind a paywall for me, I will answer these questions using the React Docs for "Components and Props"

### Question Answers: 

- *What is “props” short for?* 
    - properties

- *How are props used in React?*
    - They are used to pass data into an individual component.

- *What is the flow of props?*
    - Top down, from parent to child component. 