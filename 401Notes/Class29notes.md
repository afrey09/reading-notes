Advanced State with Reducers

Extracting State Logic into a Reducer

What is the motivation for adding a reducer? To consolidate all the state update logic outside your component in a single function - a reducer.


What are actions in the context of a reducer? How are they different than setting state directly?

  "Reducers are a different way to handle state. You can migrate from useState to useReducer in three steps:

      1. Move from setting state to dispatching actions.
      2. Write a reducer function.
      3. Use the reducer from your component."
  
 Actions are dispersed by the event handlers and are used to specify "what the user just did". When setting state directly, you are telling React what to do.

What common list operation is useReduce named for, and why? reduce()
  "The function you pass to reduce is known as a “reducer”. It takes the result so far and the current item, then it returns the next result. React reducers are an example of the same idea: they take the state so far and the action, and return the next state. In this way, they accumulate actions over time into state."


When should you switch from useState to useReducer? useReducer is easier for debugging purposes. UseReducer allows you to add console logs into the reducer so you're able to see every update and why it happened. UseReducer is also helpful for testing because it allows you to export and test it separately.

source:https://react.dev/learn/extracting-state-logic-into-a-reducer