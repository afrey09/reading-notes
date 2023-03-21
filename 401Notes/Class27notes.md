useState() Hook

Thinking in React

**What is a Hook? A function

Summarize the five steps of thinking in react.
State: A Component’s Memory

1. Break the UI into a component hierarchy - Wrap components and subcomponents into boxes and name them.

2. Build a static version of React - Build an app without any interactivity, or a static application. To ensure that the UI is rendered from your data model without interactivity added, you must create components that reuse other components and pass data using props.

3. Find the minimal but complete representation of UI state - Allowing the user to change the underlying data model allows for the UI to become interactive. This is done through using state.

4. Identify where your stat should live - Determine which component is responsible for changing the state or that owns the state. Potential locations:
  1. "Often, you can put the state directly into their common parent."
  2. "You can also put the state into some component above their common parent."
  3. "If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component."

5. Add inverse data flow - In order to change the state when there is user input, you have to support data flowing the other way: the form components deep in the hierarchy need to update the state in the table.

What is one reason a local variable isn’t sufficient for managing a React component?Local variables don't persist between renders.

What is the argument to the useState hook, and what are the two parts of its return array? The initial value of your state is the argument to the useState hook. The two parts of the return array are the state variable (index) and the state setter function (setIndex). Index is the value we stored  and setIndex can update the state variable and trigger React to render the component again.

How can Component A access state from Component B? Through the use of props. Functions from one component can be passed to another through props, which then allows the second component, or component B, to update the state of component A.

sources:
https://react.dev/learn/thinking-in-react
https://react.dev/learn/state-a-components-memory