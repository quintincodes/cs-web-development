
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: CSS_Variables
---

#reference #css

created: 1724136459110
updated: 1738275940428
---


<!--#region styles-->

<!--#endregion-->

# CSS Variables

## What Are CSS Variables?

CSS variables, also known as _Custom Properties_, allow you to store values that you can reuse throughout your CSS. They make your code cleaner, more maintainable, and easier to update.

### Syntax

CSS variables are defined using the `--` prefix and are accessed using the `var()` function.

-   <b>Defining a variable</b>
    To define a variable, you need to use the `--` prefix followed by the variable name and the value you want to assign to it. You can define variables in the `:root` pseudo-class to make them available globally.

    ```css
    :root {
        --primary-color: #3498db;
        --secondary-color: #2ecc71;
        --padding: 10px;
    }
    ```

-   <b>Using a variable</b>
    To use a predefined variable, you can use the `var()` function as a value for a CSS property.

    ```CSS
    header {
    background-color: var(--primary-color);
    padding: var(--padding);
    }
    ```

    ```CSS
    button {
        color: var(--secondary-color);
    }
    ```

It is good practice to add a <b>fallback value</b> to the `var()` function in case the variable is not defined.

```CSS
button {
    color: var(--secondary-color, #333);
}
```