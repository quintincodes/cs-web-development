
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Attributes
---

#reference #html

created: 1719484492258
updated: 1729022083990
---




## Overview and Categorization of HTML Attributes

### General Overview

HTML attributes provide additional information about HTML elements. Attributes are typically applied to elements to control their behavior and appearance. Attributes can be categorized based on their functionality and the elements they are commonly associated with. This helps in quickly identifying and using the relevant attributes.

### Common Attributes

These attributes are frequently used across multiple HTML elements.

#### `id`

-   <b>Description:</b> Specifies a unique id for an HTML element.

-   <b>Elements:</b> All HTML elements
-   <b>Posible Values:</b> Any string that uniquely identifies the element within the document.
-   <b>Syntax:</b> `id="elementId"`
-   <b>Example:</b>
    ```html
    <div id="uniqueId"></div>
    ```

#### `class`

-   <b>Description:</b> Specifies one or more class names for an HTML element.

-   <b>Elements:</b> All HTML elements
-   <b>Possible Values:</b> Any string that represents the class name.
-   <b>Syntax:</b> `class="className1 className2"`
-   <b>Example:</b>
    ```html
    <div class="className1 className2"></div>
    ```

#### `style`

-   <b>Description:</b> Specifies an inline CSS style for an HTML element.

-   <b>Elements:</b> All HTML elements
-   <b>Possible Values:</b> Any valid CSS property-value pair. Multiple properties can be separated by a semicolon.
-   <b>Syntax:</b> `style="property:value;"`
-   <b>Example:</b>
    ```html
    <div style="color:red; font-size:16px;"></div>
    ```

### Element-Specific Attributes

These attributes are grouped based on the elements they are most commonly associated with.

#### Images

-   <b>`src`<b>

    -   <b>Description:</b> Specifies the source or path of the image.

    -   <b>Possible Values:</b> URL or path to the image file.
    -   <b>Syntax:</b> `src="path/to/image"`
    -   <b>Example:</b>
        ```html
        <img src="path/to/image.jpg" alt="Image description" />
        ```

-   <b>`alt`<b>

    -   <b>Description:</b> Provides a text description of an image if it can't be displayed; used by screen readers.

    -   <b>Syntax:</b> `alt="description"`
    -   <b>Possible Values:</b> Any text description.
    -   <b>Example:</b>
        ```html
        <img src="path/to/image.jpg" alt="Image description" />
        ```

-   <b>`width`<b>

    -   <b>Description:</b> Specifies the width of an image.

    -   <b>Syntax:</b> `width="pixels|percentage"`
    -   <b>Possible Values:</b> Numeric value in pixels or percentage.
    -   <b>Example:</b>
        ```html
        <img src="path/to/image.jpg" width="100" />
        ```

-   <b>`height`<b>

        -   <b>Description:</b> Specifies the height of an image.

        -   <b>Syntax:</b> `height="pixels|percentage"`
        -   <b>Possible Values:</b> Numeric value in pixels or percentage.
        -   <b>Example:</b>
            ```html
            <img src="path/to/image.jpg" height="100" />
            ```

-   <b>`title`<b>

    -   <b>Description:</b> Provides a title or tooltip for an image.

    -   <b>Syntax:</b> `title="tooltip"`
    -   <b>Possible Values:</b> Any text that represents the tooltip.
    -   <b>Example:</b>
        ```html
        <img src="path/to/image.jpg" title="Image tooltip" />
        ```

#### Links

-   <b>`href`<b>

    -   <b>Description:</b> Specifies the link destination.

    -   <b>Syntax:</b> `href="URL"`
    -   <b>Possible Values:</b> URL or path to the linked document.
    -   <b>Example:</b>
        ```html
        <a href="https://github.com/Eddking-QS">My GitHub</a>
        ```

-   <b>`target`<b>

    -   <b>Description:</b> Specifies where the linked document will open, e.g., in a new tab, same tab, parent frame, or full window.

    -   <b>Syntax:</b> `target="_blank|_self|_parent|_top"`
    -   <b>Possible Values:</b> `_blank`, `_self`, `_parent`, `_top`.
    -   <b>Example:</b>
        ```html
        <a href="https://github.com/Eddking-QS" target="_blank">My GitHub</a>
        ```

#### Forms

-   <b>`action`<b>

    -   <b>Description:</b> Indicates where the form data should be sent.

    -   <b>Syntax:</b> `action="URL"`
    -   <b>Possible Values:</b> URL or path to the server-side script that processes the form data.
    -   <b>Example:</b>
        ```html
        <form action="submit.php"></form>
        ```

-   <b>`method`<b>

    -   <b>Description:</b> Specifies the HTTP method (GET or POST) to be used when submitting the form.

    -   <b>Syntax:</b> `method="GET|POST"`
    -   <b>Possible Values:</b> `GET`, `POST`.
    -   <b>Example:</b>
        ```html
        <form action="submit.php" method="POST"></form>
        ```

#### Input

-   <b>`type`<b>

    -   <b>Description:</b> Specifies the type of input.

    -   <b>Syntax:</b> `type="text|password|..."`
    -   <b>Possible Values:</b> `text`, `password`, `submit`, `reset`, `radio`, `checkbox`, `file`, `email`, `number`, `date`, `url`, `tel`, `search`, `color`, `range`, `time`, `datetime-local`, `month`, `week` etc.
    -   <b>Example:</b>
        ```html
        <input type="text" />
        ```

-   <b>`name`<b>

    -   <b>Description:</b> Specifies the name of the input field; used to identify form data after submission.

    -   <b>Syntax:</b> `name="fieldName"`
    -   <b>Possible Values:</b> Any string that represents the field name.
    -   <b>Example:</b>
        ```html
        <input type="text" name="firstname" />
        ```

-   <b>`value`<b>

    -   <b>Description:</b> Specifies the value of the input field.

    -   <b>Syntax:</b> `value="submitValue"`
    -   <b>Possible Values:</b> Any string that represents the field value.
    -   <b>Example:</b>
        ```html
        <input type="submit" value="Submit" />
        ```

-   <b>`placeholder`<b>

    -   <b>Description:</b> Provides a short hint that describes the expected value of an input field.

    -   <b>Syntax:</b> `placeholder="hint"`
    -   <b>Possible Values:</b> Any string that represents the hint.
    -   <b>Example:</b>
        ```html
        <input type="text" placeholder="Enter your name" />
        ```

-   <b>`required`<b>

    -   <b>Description:</b> Specifies that an input field must be filled out before submitting the form.

    -   <b>Syntax:</b> `required`
    -   <b>Possible Values:</b> None
    -   <b>Example:</b>
        ```html
        <input type="text" required />
        ```

#### Buttons

-   <b>`type`<b>

    -   <b>Description:</b> Specifies the type of button (submit, reset, or button).

    -   <b>Syntax:</b> `type="submit|reset
    -   <b>Possible Values:</b> `submit`, `reset`, `button`.
    -   <b>Example:</b>
        ```html
        <button type="submit">Submit</button>
        ```

-   <b>`disabled`<b>

    -   <b>Description:</b> Specifies that a button should be disabled.

    -   <b>Syntax:</b> `disabled`
    -   <b>Possible Values:</b> None
    -   <b>Example:</b>
        ```html
        <button type="submit" disabled>Submit</button>
        ```

#### Form Elements

-   <b>`Role`<b>

    -   <b>Description:</b> Specifies the role of the element.

    -   <b>Syntax:</b> `role="roleName"`
    -   <b>Possible Values:</b> `button`, `checkbox`, `combobox`, `grid`, `link`, `listbox`, `menu`, `menuitem`, `option`, `radio`, `searchbox`, `slider`, `spinbutton`, `switch`, `tab`, `textbox`, `tree`, `treeitem`, etc.
    -   <b>Example:</b>
        ```html
        <button role="button">Submit</button>
        ```

-   <b>`aria-label`<b>

    -   <b>Description:</b> Specifies a label for an element when the visible label is not present.

    -   <b>Syntax:</b> `aria-label="label"`
    -   <b>Possible Values:</b> Any string that represents the label.
    -   <b>Example:</b>
        ```html
        <button aria-label="Submit">Submit</button>
        ```

-   <b>`aria-labelledby`<b>

    -   <b>Description:</b> Specifies the id of another element that serves as the label for this element.

    -   <b>Syntax:</b> `aria-labelledby="elementId"`
    -   <b>Possible Values:</b> ID of another element.
    -   <b>Example:</b>
        ```html
        <button aria-labelledby="labelId">Submit</button>
        ```

-   <b>`aria-describedby`<b>

    -   <b>Description:</b> Specifies the id of another element that provides a description for this element.

    -   <b>Syntax:</b> `aria-describedby="elementId"`
    -   <b>Possible Values:</b> ID of another element.
    -   <b>Example:</b>
        ```html
        <button aria-describedby="descriptionId">Submit</button>
        ```

### Global Attributes

These attributes can be applied to any HTML element.

-   <b>`title`<b>

    -   <b>Description:</b> Provides a title or tooltip for an element.

    -   <b>Syntax:</b> `title="tooltip"`
    -   <b>Possible Values:</b> Any text that represents the tooltip.
    -   <b>Example:</b>
        ```html
        <div title="Element tooltip"></div>
        ```

-   <b>`accesskey`<b>

    -   <b>Description:</b> Specifies a keyboard shortcut to activate or focus an element.

    -   <b>Syntax:</b> `accesskey="key"`
    -   <b>Possible Values:</b> Any single character.
    -   <b>Example:</b>
        ```html
        <button accesskey="s">Submit</button>
        ```

-   <b>`contenteditable`<b>

    -   <b>Description:</b> Specifies whether the content of an element is editable.

    -   <b>Syntax:</b> `contenteditable="true|false"`
    -   <b>Possible Values:</b> `true`, `false`.
    -   <b>Example:</b>
        ```html
        <div contenteditable="true">Editable content</div>
        ```

-   <b>`draggable`<b>

    -   <b>Description:</b> Specifies whether an element is draggable.

    -   <b>Syntax:</b> `draggable="true|false"`
    -   <b>Possible Values:</b> `true`, `false`.
    -   <b>Example:</b>
        ```html
        <div draggable="true">Drag me</div>
        ```

-   <b>`hidden`<b>

    -   <b>Description:</b> Specifies that an element is not yet, or is no longer, relevant.

    -   <b>Syntax:</b> `hidden`
    -   <b>Possible Values:</b> None
    -   <b>Example:</b>
        ```html
        <div hidden>Hidden content</div>
        ```

-   <b>`aria-hidden>`<b>

        -   <b>Description:</b> Specifies whether an element is visible or hidden to assistive technologies.

        -   <b>Syntax:</b> `aria-hidden="true|false"`
        -   <b>Possible Values:</b> `true`, `false`.
        -   <b>Example:</b>
            ```html
            <div aria-hidden="true">Hidden content</div>
            ```