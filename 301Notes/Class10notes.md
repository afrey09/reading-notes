JavaScript Call Stack

1. The call is the function invocation or what is used to execute the function code

2. Only one can happen at a time

3. LIFO - Last In First Out - "the last function that gets pushed into the stack is the first to be pop out, when the function returns"

4. 

5. Stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.

Source:https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4


JavaScript Error Messages

1. Reference error: Can happen when you try to use a variable that is not yet declared or to let and const when they are hoisted but there is a temporal dead zone between being hoisted and being declared

2. Syntax error: Happens when you have something that cannot be parsed in terms of syntax.

3. Range error: When you try to manipulate some kind of length and give it an invalid length

4. Type error: Shows up when the types (number,string and so on)you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

5. Breakpoint: Used when you add a debugger statement in your code in the line you want to break. It will make your program stop at that point, only if a condition is met.

6. Debugger (Can be run by pressing F5) - Used on the line of code that you want to create a breakpoint

Source:https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c
