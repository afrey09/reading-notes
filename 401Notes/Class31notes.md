CONTEXT API

Choosing the State Structure

Summarize the five principles for structuring state.

  1. Group related state. If you always update two or more state variables at the same time, consider merging them into a single state variable.
  2. Avoid contradictions in state. When the state is structured in a way that several pieces of state may contradict and “disagree” with each other, you leave room for mistakes. Try to avoid this. 
  3. Avoid redundant state. If you can calculate some information from the component’s props or its existing state variables during rendering, you should not put that information into that component’s state.
  4. Avoid duplication in state. When the same data is duplicated between multiple state variables, or within nested objects, it is difficult to keep them in sync. Reduce duplication when you can.
  5. Avoid deeply nested state. Deeply hierarchical state is not very convenient to update. When possible, prefer to structure state in a flat way.


Passing State Deeply with Context

What problem do Contexts aim to solve? Needing to pass data to the components without the use of props. If the component is several levels deep within the tree or there are several components needing the data, "lifting state up that high can lead to a situation called, 'prop drilling'."


What is one technique to try before useContext? To try to pass props if there are not several components 


What hook complements useContext for complex applications? useReducer

source: 
https://react.dev/learn/passing-data-deeply-with-context
https://react.dev/learn/choosing-the-state-structure