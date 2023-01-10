React Lifecycle

- Based off the diagram, the "render" happens before the "componentDidMount" both during Mounting and Unmounting 

- The very first thing to happen in the lifecycle of React is the constructor and occurs in Mounting

- constructor
  render
  componentDidmout
  componentDidUpdates
  componentWillUnmount

-  componentDidMount : "A method invoked immediately after a component is mounted." Used when needing to load anything using a network request or if you want to initialize the DOM. Also used to "connect to the YouTube API and get videos when the components is rendered."

React State vs. Props

"Props are like arguments to a function... things you want to pass to a function"
"State is something inside of a component" 

States can be changed within the component but props must be changed on the outside of the component. States are used to update the application based on user input. Ex. Forms

If information is static, use props.


- Props are like the arguments to a function but for a component. Ex. A title and description that you want to be rendered from a component. They are used when you don't want to hard code something and are more like variables.

- "Main difference between states and props is that props are PASSED INTO a component and state is handled inside of that component. And props are handled outside the component"

- We re-render our application as the input changes. We use states to re-render and update based on something the user has done.

- The example mentioned in the video is the counter. We need the state to store the thing that we are going to be updating.


Sources: https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093
         https://www.youtube.com/watch?v=IYvD9oBCuJI&themeRefresh=1
