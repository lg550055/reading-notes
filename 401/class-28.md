# Django Forms

Use forms to create, update, and delete model instances.

HTML forms allow us to collect user input in different formats, including text boxes, checkboxes, radio buttons, date pickers, etc.

HTML forms, using the POST method, are a relatively secure way to send data to the server.

> Django Forms provide a framework to define forms and their fields programmatically, and use these objects to generate the form HTML code and handle much of the validation and user interaction.

### Form handling

> The view gets a request, performs any actions required including reading data from the models, then generates and returns an HTML page (from a template, into which we pass a context containing the data to be displayed).

1. Display default form the first time it is requested (GET request)
2. Receive data from a submit request and bind it to the form (POST request)
3. Clean and validate the data
4. If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields
5. If all data is valid, perform required actions, then redirect as appropriate

### Form class

> The Form class handles forms. It specifies the fields, their layout, display widgets, labels, initial values, valid values, and (once validated) the error messages associated with invalid fields.  It also provides methods for rendering or for getting the value of any element.

Declaring a form is very similar to declaring a model.  Use the same field types and similar parameters.

The form class lives in the file forms.py.  It inherits from the forms.Form Django class.

### Create a form using ModelForms

Use the ModelForm class to map fields, labels, etc. from your models to your forms.

### Generic editing views

In its views.generic.edit model Django provides a CreateView, UpdateView and DeleteView to simplify the implementation of these common operations.

---

### Resources

- [Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)
- [Django Templates](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)
- [Django Views](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)

---

[Back to table of contents](../README.md)