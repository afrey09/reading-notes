HTML

Ordered and Unordered Lists

  Unordered is represented by ul and is for grouping a collection of items together that do not have a numerical order to them and it does not matter where each item falls in a list

  Ordered is represented by ol and should be used when the order of items being changed effects the meaning

  To change the bullet style of a list, use the attribute "type". The bullet style is not definted in HTML but in CSS, use the list-style-type property

  Use an ordered list only if the position change of the items within the list effect the intended meaning. If not, use ul

  To change numbers on a list item,you can use the "start" attribute. For example ol start = 4 if you want the list to start at number 4. You can also use nesting to have unordered within ordered lists or vice versa

  CSS

  Margin and padding work together to create box you can see on the page. It plays a part in the sizing of the box but indirectly and only externally.
  
  The Box Model

    Content box - The area where your content is displayed; size it using properties like inline-size and block-size or width and height

    Padding box - Sits around the content as white space; size it using padding and related properties

    Border box - Wraps the content and any padding; size is using border and related properties

    Margin box - The outermost layer, wrapping the content, padding and border as whitespace between this box and other elements; size it using margin and related properties

    Learn JS

    Arrays, Operators and Expressions, Conditionals, Loops

    Arrays - Data type/structure- collection or list of elements; single objects that contain multiple values stored in a list. Can be stored in variables. You don't have to determine the size it will be. Data types that can be stored include: strings, numbers, objects and other arrays. Multiple types can be stored within on array. Every element will have a position in array that's referred to as it's index. Arrays are zero based index

    Built-in methods:
      `.push()` - add to the end of the array
      `.pop()` - removed the last element from an array

      `.length` - tells you how many elements live in the array

    People array is not valid. Alternatively you could use names.
    To access individual items in an array, use bracket notation and supply the items index in the same way you access letters in a string

    5 Shorthand operators for assignment in JS:

        X = f () - assignment
        X  += f () - addition assignment
        X -= f () -subtraction assignment
        X *= f () - multiplaction
        X <<= f () - left shift assignment 

    Evaluating the expression - Need additional guidance

    A real world example of when a conditional statement should be used in JS program would be if you are creating a for loop and need to make an if else statement.

    A loop is useful in JS if you are needing to gather certain input or information from the user. For example when I website would like your email address to add to their mailing list before they'll let you view the website's content

