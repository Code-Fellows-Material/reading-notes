# Class 02 Reading Notes

## Things I want to know more about

## React Life Cycle

- **Link:** [React: Component Lifecycle Events, by Joshua Blankenship](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
\
![Component Life Cycle](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)
\ 
- **Link to React Documentation over same subject (more detailed and comprehensible):** [react-component docs](https://reactjs.org/docs/react-component.html)
- See cleaner diagram [HERE](https://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/)

### Question Answers: 

- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
    - *render happens before componentDidMount()*

- What is the very first thing to happen in the lifecycle of a React component?
    - *The constructor is called*
    
- Put the following things in the order that they happen: 

    - `constructor`
    - `render`
    - `componentDidMount`
    - `React Updates` component receives new props, setState() or forceUpdate() is called.
    - + `render` component re-renders after update
    - + `componentDidUpdate` called after updating happens
    - `componentWillUnmount`

- What does componentDidMount do?

    - *componentDidMount is called after a component is mounted (its usually a good place to make a network request)*

####: Side Notes

- See React Docs link above for more detailed info.