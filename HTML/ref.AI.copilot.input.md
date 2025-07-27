
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: input
---

#reference #html

created: 1719676084276
updated: 1724443609716
---




## HTML Form Elements Reference

-   <b>Labels and Input Controls</b>

-   Labels are crucial for accessibility and usability in forms. They provide a textual description for form inputs, making forms navigable by screen readers and other assistive technologies.
-   An input control refers to any form element that allows users to enter data. This includes text fields, checkboxes, radio buttons, and more.
-   Always use the `<label>` element to ensure form elements are accessible. The `for` attribute of the label should match the `id` of the input control it describes.
-   Example with Label:

    ```html
    <label for="age">Age:</label> <input type="text" id="age" name="age" />
    ```

-   <b>Fieldset and Legend</b>

-   The `<fieldset>` element is used to group related elements within a form. It enhances both the organization of the form and its accessibility.
-   The `<legend>` element provides a caption for the `fieldset`, helping users understand the context of the grouped inputs.
-   Example of Fieldset and Legend:

    ```html
    <fieldset>
        <legend>Contact Information</legend>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" />
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" />
    </fieldset>
    ```

    ### Input Types

HTML provides various input types to cater to different data entry requirements. Some common input types include:

-   `text`: Single-line text input. This is the default type for input elements.
-   `password`: Password input (characters are masked).
-   `email`: Email address input with validation. If the input does not match the email format, the form will not submit.
-   `checkbox`: Checkbox for selecting multiple options. Multiple checkboxes can be selected. The `value` attribute specifies the value submitted when the checkbox is checked.
-   `radio`:

Radio button for selecting a single option from a group. The `value` attribute specifies the value submitted when the radio button is selected. All radio buttons within the same group should have the same `name` attribute.

-   `submit`: Button to submit the form.
-   `reset`: Button to reset the form.
-   `file`: File upload input.
-   `date`: Date input.
-   `number`: Number input.
-   `range`: Range input (slider).
-   `color`: Color picker input.
-   `tel`: Telephone number input.
-   `url`: URL input.
-   `search`: Search input.

-   Example of Input Types:

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username" />
<label for="password">Password:</label>
<input type="password" id="password" name="password" />
<label for="email">Email:</label>
<input type="email" id="email" name="email" />
<label for="age">Age:</label>
<input type="number" id="age" name="age" />
<input type="checkbox" id="subscribe" name="subscribe" />
<label for="subscribe">Subscribe to Newsletter</label>
```

-   <b> Input id and name Attributes</b>

-   The `id` attribute uniquely identifies an element within a document. It is used to associate a label with a form control.
-   The `name` attribute specifies the name of the input control when the form is submitted.
-   Example of Input id and name Attributes:
    ```html
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" />
    ```