Component Lifecycle/useEffect Hook

1. What is the main intended use case for the useEffect hook?
The useEffect hook allows you to connect to an external system such as a browser API, a third-party library or another network. 

2. How does the effect’s logic interact with the component? By "allowing you to keep your component synchronized with some external system." It should "mirror" the setup logic: mount, update, unmount. This allows the effect to withstand the setup and cleanup running by React as often as needed. 

3. What is the importance of the return value from the effect’s logic function? It is used for cleanup purposes which allows you to disconnect, unsubscribe, etc. 

source: https://react.dev/reference/react/useEffect#reference

ReadMe

1. I would like to understand useEffect more thoroughly and see it implemented into an application so I can get a better grasp on how it changes the code.