Async Actions

1. Why use Redux middleware? Redux middleware allows us to do things like make asynchronous requests to an API.

2. Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.
  An event handler dispatches an action/thunk to the middleware which then sends an asychronous request to the API. The API returns a response which is then sent to the reducer which updates the state. The state is then sent to the store which updates the UI.

3. How are we accomodating async in our Redux app? We are using Redux Thunk to handle async actions by sending it to the middleware.

source: https://redux.js.org/tutorials/fundamentals/part-6-async-logic

Thunk Middleware

1. Why would you need redux-thunk middleware? "It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods."

2. Redux Thunk middleware allows you to write action creators that return a ___function___ instead of an action.

3. Describe how any return value from the inner thunk function will be made available. "Any return value from the inner function will be available as the return value of dispatch itself. This is useful for orchestrating an asynchronous control flow with thunk action creators dispatching each other and returning Promises to wait for each other's completion."

source:https://github.com/reduxjs/redux-thunk
