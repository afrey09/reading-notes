Functional Programming

1. "Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia"

2. Pure function definition and two parameters for being considered pure:

  - It returns the same result if given the same arguments (it is also referred as    deterministic)
  - It does not cause any observable side effects

3. Benefits of pure function:

  - The code is easier to test
  - You don't have to mock anything

4. Immutability: unchanging over time or unable to be changed

5. Referential Transparency: When a function consistently yields the same result for the same input

Source: https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa

1. Module - Used to break up the code into differently pieces with different functionality. It is essentially just another JavaScript file.

2. Require - used to create a path to the module that is needed. 
      Syntax: require('./name);

3. To bring a module into the file you're working in, the module has to be set to export.. Ex. module.exports = counter. Then from the file you're working in, you use the require('./count) but set to a variable called counter. 
    
      var counter = require(./count)

4. To make a module available, you have to export it from the module. Ex. module.exports = counter

Source: https://www.youtube.com/watch?v=xHLd36QoS4k


