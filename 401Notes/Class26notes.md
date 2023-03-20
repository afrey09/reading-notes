React Quick Start

Read the React Quick Start quide, to refresh your memory on React.

What are the building blocks of a React app?
  Components

What is the difference between an HTML element and a React component?
  HTML elements are always lowercase while React components are always capitalized

What is JSX and why do we use it?
  JSX is the preferred markup syntax for React applications. JSX is convenient and accepted by most of the tools recommended for development.

Describe the process of embedding JavaScript expressions in JSX.
  "JSX lets you put markup into JavaScript. Curly braces let you “escape back” into JavaScript so that you can embed some variable from your code and display it to the use...You can also “escape into JavaScript” from JSX attributes, but you have to use curly braces instead of quotes. For example, className="avatar" passes the "avatar" string as the CSS class, but src={user.imageUrl} reads the JavaScript user.imageUrl variable value, and then passes that value as the src attribute."

Does React or JSX have any special features for iteration or conditional logic? The map() method for iteration and the ternary operator for conditional logic


How does React know to respond to a user’s inputs? Through the use of event handlers


What word indicates that a React component manages data with a Hook? "Use"


How can two react components share data? Through the use of props between the components 


Render and Commit

What are the three steps of refreshing a React UI?
  - Trigger
  - Render
  - Committing to the DOM 

How do you trigger updates to a component after the initial render? using the set function


Does React recreate DOM nodes on every rerender? No, it only rerenders the nodes that need rerendering 


After React has updated the DOM, what still needs to happen before the user sees the change? The browser needs to render the new content ("paint the screen")

Sources: https://react.dev/learn
https://react.dev/learn/render-and-commit
