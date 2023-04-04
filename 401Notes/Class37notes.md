Redux - Combine Reducers

Multiple Reducers Example

Why create multiple reducers? To keep your code organized and to make it easier to manage.

How would you combine multiple reducers? through the use of combineReducers. Once combined, you can pass each reducer its specific state information. Once modified, the new state is returned and passed to the store.

How will you manage state as an immutable object? By using the spread operator to create a new object with the updated information. Why? Because the spread operator creates a new object, and does not modify the original object.

Redux Docs: Using Combined Reducers

combineReducers is a utility function to simplify the most common use case when writing Redux reducers. 

Explain how combineReducers assembles the new state tree. It takes in an object with reducers as values and returns a function that will call each reducer with the state and action.

How would you define initial state in an app using combineReducers? You would define the initial state in each reducer. Then you would pass the initial state to the combineReducers function.

Redux Docs: Combined Reducer Syntax

Why will you want to split your reducing functions as your app becomes more complex? To keep your code organized and to make it easier to manage state.

The __combineReducers___ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to __createStore__.

What is a popular convention when naming reducers? To name them after the state they manage.

source:https://redux.js.org/usage/structuring-reducers/using-combinereducers/
https://redux.js.org/api/combinereducers/
https://www.youtube.com/watch?v=gBER4Or86hE