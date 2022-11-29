Intro to HTML

  Semantic elements are important because provide meaning and structure to text so that a browser is able to display the information properly

  There are 6 heading elements in HTML <h1>-<h6>

  Superscript <sup> and subscript <sub> are used "when marking up items like dates, chemical formulae, and mathematical equations so they have correct meaning"

  Title is the full expansion of the term <abbr>. Example <abbr title>

CSS Structure

  To apply CSS to HTML, you have three options: using an external stylesheet, with an internal stylesheet or with inline styles
  Inline styling is not recommended because it is a less efficient way of working. It also makes things more difficult to read and understand because it mixes presentational code (CSS) with HTML.A scenario where it might be useful would be if you were blocked from modifying an external CSS file
  BLOCK OF CODE:
      h2 {
        color: black;
        padding:5px;
      }
      Questions - 
          The selector is h2
          The declarations are both the properties and their values, black and 5px
          The properties are color and padding

  Learn JS

    The data type that is a sequence of text enclosed in single quote marks is a 'String'
    4 JS Operator Types:
      Addition +
      Assignment =
      Strict equality ===
      Not, Does-not-equal !, !==

    A real world problem that could be solved with a function would be determining how many miles a car has driven (output) which is based on how long the car has been driving (input)

  Making Decisions in Your Code - Conditionals

      An if statement checks a condition and if it evaluates to true, the code block will execute
      The purpose of an else if statement is so that if the statement is not true, or the condition is false, a different code will run
      3 Types of Comparison Operators:
        === and !==
        < and >
        <= and >=
      The difference between && and || is && is AND and || is OR. And allows you to chain together two or more expressions so that all of them have to evaluate to true individually for the whole expression to be true. OR allows you to chain together two or more expressions so that only one or more of them have to individually evaluate to true for the whole expression to be true