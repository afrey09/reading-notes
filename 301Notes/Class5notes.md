Thinking in React

1. The idea that a component should ideally only do one thing and if it grows, should be decomposed into smaller subcomponents.

2. It is where you build a version that takes your data model and renders the UI but does not have any interactivity.

3. Once you have a static application, you need to then add state.

4. Three questions to ask to determine is something is state:
    -Is it passed in from a parent via props? If so, it probably isn’t state.
    -Does it remain unchanged over time? If so, it probably isn’t state.
    -Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. To identify where each piece of state in your application needs to live:

    -Identify every component that renders something based on that state.
    -Find a common owner component (a single component above all the components that need the state in the hierarchy).
    -Either the common owner or another component higher up in the hierarchy should own the state.
    -If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component

Source:https://reactjs.org/docs/thinking-in-react.html

Higher-Order Functions

1. Definition: "Functions that operate on other functios, either by taking them as arguments or by returning them."

2. It is returning a value greater than the property defined in the greaterThan function

3. Reduce: "It builds a value by repeatedly taking a single element from the array and combining it with the current value."

   map: "The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function."

Source:https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK
