Passing Functions as Props

1. map() returns a new array
2. In React, to loop through and array and display each value in JSX, the map() function. Returned is a <li> element for each item.
3. Each list item needs a unique KEY
4. Keys are used to help React identify items that have been modified, removed or added. "Keys should be given to the elements inside the array to give the elements a stable identity."

Source: https://reactjs.org/docs/lists-and-keys.html

The Spread Operator

1. "The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments...refers to the use of an ellipsis of three dots(...) to expand an iterable object into the list of arguments."
2. Things it can do:
    - spread arrays into separate arguments
    - copy arrays
    - concatenate or combine arrays
    - use math functions
    - add an item to a list
    - use arrays as arguments
    - add to state in React
    - combine objects
    - convert NodeList to an array
3. Combining example:
    
    const myArray = [`🤪`,`🐻`,`🎌`]
    const yourArray = [`🙂`,`🤗`,`🤩`]
    const ourArray = [...myArray,...yourArray]
    console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
4. Adding a new item example:
    
    const fewFruit = ['🍏','🍊','🍌']
    const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
    console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
5. Combing two objects into one example:

    const objectOne = {hello: "🤪"}
    const objectTwo = {world: "🐻"}
    const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
    console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
    const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
    objectFour.laugh() // 😂😂😂😂😂
    


Source: https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab
