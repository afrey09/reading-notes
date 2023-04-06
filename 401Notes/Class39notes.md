Redux Toolki

1. What concerns are addressed by Redux Toolkit? Redux Toolkit was created initially to help three common Redux concerns:
  
      - "Configuring a Redux store is too complicated"
      - "I have to add a lot of packages to get Redux to do anything useful"
      - "Redux requires too much boilerplate code"

2. What does configureStore() do? "configureStore(): wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension." 

3. How would I use createSlice()? createSlice() is a function that accepts an initial state, an object full of reducer functions, and a "slice name" and automatically generates action creators and action types that correspond to the reducers and state.

source: https://redux-toolkit.js.org/introduction/getting-started

MobX

1. What is mobX? "A simple, scalable and battle tested state management solution." It is considered a standalone library but is most commonly used with React.

2. How does MobX make it "impossible" to produce an inconsistent state? It makes sure that everything that can be derived from the application state, will be derived. Automatically.

3. How would you build a reactive user interface? Through the use of the observer function which wraps the React component in autorun.This will make sure that the component is re-rendered whenever the data it uses changes.

source:https://mobx.js.org/getting-started.html

