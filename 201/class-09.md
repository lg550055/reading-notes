# Forms and JS Events
Forms and Events are essential to collect user information.

## Forms
Forms allow a user to enter information into a web application.

#### Form Controls
Form fields have a 'name' and the user enters a 'value', both of which on 'submit' get passed on to the backend

- Text 
  - Text input -single line of text
  - Text area -multi-line text
  - Password -characters masked
- Choices
  - Radion buttons -select one option
  - Checkboxes -select multiple options
  - Drop-down (aka `select`) -pick one from a list
- Submit
  - Submit button
  - Submit image -similar to button but with image
- Flie upload

#### Form Stucture
Form controls live inside a `<form>` element, which always carries the `action` attribute.

###### `<form>` Attributes
- `action` value: location on the backend receiving the information on submit
- `method` value: `get` or `post`
  - `get` -for retrieving information (value is attached to url)
  - `post` -for submiting information

###### `<input>` Attributes
- name: tells the server from which form control the data was entered
- type
  - text
    - size (deprecated)
    - maxlength (# of chars user may enter)
  - password -may use maxlength
  - radio
    - value -value sent to backend for this option
    - checked -default option
  - checkbox
    - value -value sent to backend for this option
    - checked -default option
  - select (uses `<select>` instead of input)
    - `<option>`
      - value -sent to backend...
      - selected -default option
  - date (HTML5)
  - email (HTML5)
  - url (HTML5)
  - search (HTML5)

*Use `placeholder` attribute on any text input: text, password, email, url, search*

### Form Validation
Form validation, an HTML5 feature, alerts the user if the form control has not been filled in correctly.

For example: `<input> required="required"...`


---

## JS Events intro
An Event is an action that takes place in the DOM.

Events can be triggered by:
- User action,
- APIs
- Programmatically

There are many types of events.

>Many DOM elements can 'listen' for events, and
>'handle' (execute code to process) them

>Event 'handlers' are usually 'attached' to other DOM elements


---

[Back to table of contents](../README.md)
