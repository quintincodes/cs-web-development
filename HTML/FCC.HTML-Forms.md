
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: HTML-Forms
---

#freecodecamp #tutorial #html

created: 1720780667296
updated: 1724443609719
---




## Using HTML Forms

HTML forms are a way to collect data from users. For example, login forms, registration forms, and feedback forms are all types of forms. <b>The form element</b> in HTML is used to create a form. This element has an <b>action attribute</b> that specifies where the form data should be sent. It also has a <b>method attribute</b> that specifies how the form data should be sent.

### The `<form>` Element

The form element is a container for different types of input elements, such as text fields, checkboxes, radio buttons, submit buttons, etc. The form element is defined by the `<form>` tag. The form element contains the following attributes:

-   <b>action :</b> The URL where the form data will be sent. This is usually a server-side script that will process the form data. eg. `action="/submit-form.php"`

-   <b>method :</b> The HTTP method used to send the form data. The most common methods are `GET` and `POST`. The `GET` method appends the form data to the URL in the form of query parameters. The `POST` method sends the form data in the body of the request. eg. `method="POST"`

## Elements Used in Forms

The following elements are commonly used in HTML forms:

-   <b>Input Elements :</b> These are used to collect data from the user. The most common input elements are text fields, checkboxes, radio buttons, and submit buttons. example: `<input type="text">`

-   <b>Label Elements :</b> These are used to provide a label for an input element. Labels help users understand what information is expected in an input field. example: `<label for="username">Username:</label>`
-   <b>Button Elements :</b> These are used to create buttons in a form. Buttons can be used to submit the form, reset the form, or trigger a custom action. example: `<button type="submit">Submit</button>`
-   <b>Select Elements :</b> These are used to create dropdown lists in a form. Users can select one option from the list. example: `<select><option value="1">Option 1</option></select>`
-   <b>Textarea Elements :</b> These are used to create multi-line text fields in a form. Users can enter multiple lines of text in a textarea element. example: `<textarea></textarea>`
-   <b>Fieldset Elements :</b> These are used to group related elements in a form. Fieldsets can be used to create sections in a form and provide a visual grouping of elements. example: `<fieldset><legend>Personal Information</legend></fieldset>`
-   <b>Legend Elements :</b> These are used to provide a caption for a fieldset element. Legends help users understand the purpose of the grouped elements. example: `<legend>Personal Information</legend>`

## Example of a Simple Form

Here is an example of a simple form that collects a username and password from the user:

```html
<form action="/submit-form.php" method="POST">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" />
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" />
    <button type="submit">Submit</button>
</form>
```

## Attributes of Form Elements

Form elements can have various attributes that control their behavior and appearance. Some common attributes used with form elements are:

-   <b>name :</b> Specifies the name of the form element. The name attribute is used to identify the form element when the form is submitted. example: `name="username"`

-   <b>id :</b> Specifies a unique id for the form element. The id attribute is used to uniquely identify the form element in the document. example: `id="username"`
-   <b>value :</b> Specifies the initial value of the form element. The value attribute is used to pre-fill the form element with a default value. example: `value="John Doe"`
-   <b>required :</b> Specifies that the form element is required. The required attribute is used to make a form element mandatory. example: `required`
-   <b>disabled :</b> Specifies that the form element is disabled. The disabled attribute is used to prevent users from interacting with the form element. example: `disabled`
-   <b>readonly :</b> Specifies that the form element is read-only. The readonly attribute is used to prevent users from editing the form element. example: `readonly`
-   <b>placeholder :</b> Specifies a short hint that describes the expected value of the form element. The placeholder attribute is used to provide a hint to users about the expected input. example: `placeholder="Enter your username"`
-   <b>maxlength :</b> Specifies the maximum number of characters that can be entered in the form element. The maxlength attribute is used to limit the length of the input. example: `maxlength="20"`
-   <b>min :</b> Specifies the minimum value of the form element. The min attribute is used to set a minimum value for number and date inputs. example: `min="0"`
-   <b>max :</b> Specifies the maximum value of the form element. The max attribute is used to set a maximum value for number and date inputs. example: `max="100"`