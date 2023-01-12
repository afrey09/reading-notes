React Docs - Forms

  "..form elements naturally keep some internal state."

  1. Controlled Component:  A React component that renders a form but also controls what happens in that form upon additional user input; an input form element.

  2. We would want to update the state with the responses as they're being typed so that the displayed value updates as the user types

  3. HandleChange(event) allows you to target what the user is entering 

  Source: https://reactjs.org/docs/forms.html
  
  Conditional (Ternary) Operator  
  
  Syntax: condition? value if true : value if false

  Typical if statement: 

    if (person.age >= 16) {
      person.driver = 'Yes';
        } else {
      person.driver = 'No';
    }

    using conditional operator: 

      person.driver = person.age >=16 ? 'Yes' : 'No';


  1. Used to shorten if statements into one line of code.

  2. if(x===y){
       console.log(true);
      } else {
      console.log(false);
    }

    using conditional operator:

      x===y ? 'true' : 'false"


  Source: https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff
