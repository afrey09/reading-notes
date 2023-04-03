Application State with Redux

What is the first principle of Redux? Single sourece of truth - The first principle of Redux is that the whole state of your application is stored in an object tree within a single store.

What is the second principle of Redux? State is read-only - The second principle of Redux is that the state is read-only. The only way to change the state is to emit an action, an object describing what happened.

Name three Redux store methods given to us by createStore and describe their use. getState - Returns the current state of the store. 
dispatch - Takes an action and returns the new state of the store. 
subscribe - Takes a callback function and returns a function that will unsubscribe the callback from the store.

Explain to a non-technical recruiter what combineReducer() does and why it's useful. combineReducer() is a function that takes an object as an argument. The object contains key/value pairs where the key is the name of the reducer and the value is the reducer function. combineReducer() returns a function that takes the state and action as arguments. The function will call the reducer function that matches the key in the object and return the new state.


source:https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867