1. What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem? 
    What data structure will be the most efficient for time and space complexity. Some data structures require more memory than other to store the same amount of data. Also taking into considering is the ease of maintenance and implementation of the data structure.


2. How can we ensure that we’ll avoid an infinite recursive call stack? 

    Ensure that your recursion has a base case: The base case is the condition that stops the recursion. Without a base case, the recursion will continue infinitely. Make sure that the base case is well-defined and that it will eventually be reached.

    Check for termination conditions: In addition to the base case, you should also check for other termination conditions that might cause the recursion to stop. These could be things like reaching a maximum depth or hitting a specific condition.

    Use tail recursion: Tail recursion is a technique where the recursive call is the last operation performed in a function. This allows the compiler or interpreter to optimize the code and avoid building up a call stack. Some programming languages have built-in support for tail recursion optimization.

    Increase the stack size: In some cases, the call stack may be too small to handle the recursion depth that you require. You can increase the stack size in your program or through system settings to allow for deeper recursion.

    Use an iterative approach: In some cases, you may be able to re-write your algorithm in an iterative way instead of using recursion. This can avoid the need for a call stack altogether and may be more efficient.