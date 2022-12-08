Class 9 Notes

1. Web forms are necessary or the preferred way of interacting with the user, especially when it comes to collecting user data.

2. When considering user experience, it is important to remember that simplicity is key and to ask only for the data absolutely needed.

3. 5 Elements and what they do:

    form - "formally defines a form and atttributes that determine the form's behavior." All forms start with the element form.

    fieldset - this element provides a "convenient way to create groups of widgets that share the same purpose, for styling and semantic purposes." 

    legend - used to label a fieldset element and included just below the fieldset upening tag. "The text content of the legend formally describes the purpose of the fieldset it is included inside."

    label - "The formal way to define a label for an HTML form widget. This is the most important element if you want to build accessible forms.

    input - Used toe create controls such as dropdown boxes, buttons, checkboxes, or radio buttons.

    texarea - the input field for a message is a texarea; a multiline text field.

4. To a non-technical friend, I would describe events are the user's actions that interact with the site. For example, when the user clicks, hovers, mouseovers or presses keys. Those are all considered events

5. When using the addEventListener, the two arguments needed are the type of event and the event handler.

6. The event object lives inside the event handler function and is the parameter that's specified with a name such as event, evt, or e. "It is automatically passed to event handlers to provide extra features and information...
The target within the event object is always a reference to the element the event occurred upon."

7. The difference between event bubbling and event capturing:

  - Event Bubbling "describes how the browser handles events targeted at nested elements." The event handler first runs on the child element, then the parent and then to the rest of the ancestors.
  - Event Capturing is the reverse of event bubbling. The event instead starts at the parent element and then to the child element.


Sources: 

  - https://developer.mozilla.org/en-US/docs/Learn/Forms
  - https://developer.mozilla.org/en-US/docs/Learn/Forms/   Your_first_form
  - https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form
  - https://developer.mozilla.org/en-US/docs/Learn/JavaScript
  - https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events

