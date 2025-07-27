
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: CSS-Basics
---

#freecodecamp #tutorial #css

created: 1719775855951
updated: 1724443609698
---




**CSS is the language used to describe how HTML elements are displayed on the screen, or any other media. It can control the layout of multiple web pages all at once.**

**<b>CSS rules</b> are made up of selectors and declarations. The selector is used to target the HTML element you want to style, and the declaration is used to specify the style you want to apply.**

**CSS can be added to HTML documents in three ways: <i>inline</i>, <i>internal</i>, and <i>external</i>.**

-   <b>Inline CSS :</b>
    This is done by adding the `style` attribute to the HTML element. The `style` attribute can contain any CSS property. The example below shows how to change the color and the font size of the paragraph element using inline CSS.

    ```HTML
    <p style="color: blue; font-size: 20px;">This is a paragraph.</p>
    ```

-   <b>Internal CSS :</b> <br>
    This is done by adding a `style` element inside the `head` section of the HTML document. The example below shows how to change the color and the font size of the paragraph element using internal CSS.

    ```HTML
    <!DOCTYPE html>
    <html>
    <head>
        
    </head>
    <body>
        <p>This is a paragraph.</p>
    </body>
    </html>
    ```

-   <b>External CSS :</b> <br>
    This is done by creating a separate CSS file and linking it to the HTML document using the `link` element. The example below shows how to change the color and the font size of the paragraph element using external CSS.

    ```HTML
    <!DOCTYPE html>
    <html>
    <head>
        <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
        <p>This is a paragraph.</p>
    </body>
    </html>
    ```

### Selectors

**CSS selectors are used to select the HTML elements that you want to style. There are several types of selectors in CSS:**

-   <b>Element Selector :</b>
    Selects all elements of a specific type. The example below shows how to change the color of all paragraph elements to blue.

    ```CSS
    p {
        color: blue;
    }
    ```

-   <b>ID Selector :</b>
    Selects an element with a specific ID. The example below shows how to change the color of the element with the ID `para1` to blue.

    ```CSS
    #para1 {
        color: blue;
    }
    ```

-   <b>Class Selector :</b>
    Selects all elements with a specific class. The example below shows how to change the color of all elements with the class `para` to blue.

    ```CSS
    .para {
        color: blue;
    }
    ```

-   <b>Attribute Selector :</b>
    Selects elements based on their attributes. The example below shows how to change the color of all `a` elements with the `href` attribute to blue.

    ```CSS
    a[href] {
        color: blue;
    }
    ```

    > <b>The following are some types of attribute selectors in CSS:</b>
    >
    > -   <i>`attribute` : Selects elements with the specified attribute. Example: `[type] { color: blue; }`</i>
    >
    > -   <i>`attribute="value"` : Selects elements with the specified attribute and value. Example: `[type=text] { color: blue; }`</i>
    >
    > -   <i> `attribute~="value"` : Selects elements with the specified attribute and a value that contains a specific word. Example: `[class~=para] { color: blue; }`</i>
    >
    > -   <i>`attribute|="value"` : Selects elements with the specified attribute and a value that starts with a specific word. Example: `[lang|=en] { color: blue; }`</i>
    >
    > -   <i>`attribute^="value"` : Selects elements with the specified attribute and a value that starts with a specific string. Example: `[href^="https"] { color: blue; }`</i>
    >
    > -   <i>`attribute$="value"` : Selects elements with the specified attribute and a value that ends with a specific string. Example: `[href$=".com"] { color: blue; }`</i>
    >
    > -   <i>`attribute*="value"` : Selects elements with the specified attribute and a value that contains a specific string. Example: `[href*="w3schools"] { color: blue; }`</i>

-   <b>Descendant Selector :</b>
    Selects an element that is a descendant of another element. The example below shows how to change the color of all `span` elements that are descendants of a `div` element to blue.

    ```CSS
    div span {
        color: blue;
    }
    ```

-   <b>Universal Selector :</b>
    Selects all elements on the page. The example below shows how to change the color of all elements on the page to blue.

    ```CSS
    * {
        color: blue;
    }
    ```

-   <b>Grouping Selector :</b>
    Selects all elements with the same style definitions. The example below shows how to change the color of all `h1`, `h2`, and `h3` elements to blue.

    ```css
    h1,
    h2,
    h3 {
        color: blue;
    }
    ```

-   <b> Pseudo-selectors :</b>
    Selects elements based on their state or position. The example below shows how to change the color of the `a` element when the mouse hovers over it.

    ```css
    a:hover {
        color: red;
    }
    ```

    > <i>To select <b>the last type of a specific</b> element, use the `:last-of-type` pseudo-class. The example below shows how to change the color of the last paragraph element to red.</i>
    >
    > ```css
    > p:last-of-type {
    >     color: red;
    > }
    > ```
    >
    > <i>To select <b>the first type of a specific</b> element, use the `:first-of-type` pseudo-class. The example below shows how to change the color of the first paragraph element to red.</i>
    >
    > ```css
    > p:first-of-type {
    >     color: red;
    > }
    > ```
    >
    > <i>To select <b>the nth type of a specific</b> element, use the `:nth-of-type(n)` pseudo-class. The example below shows how to change the color of the second paragraph element to red.</i>
    >
    > ```css
    > p:nth-of-type(2) {
    >     color: red;
    > }
    > ```
    >
    > <i>`:not(selector)` pseudo-class is used to select all elements that do not match the specified selector. The example below shows how to change the color of all elements except the `p` element to red.</i>
    >
    > ```css
    > :not(p) {
    >     color: red;
    > }
    > ```

-   <b> Child Selector :</b>
    Selects an element that is a child of another element. The example below shows how to change the color of all `span` elements that are children of a `div` element to blue.

    ```css
    div > span {
        color: blue;
    }
    ```

### Facts, Tips and Tricks

-   <b> Negative Margins :</b>
    Negative margins can be used to overlap elements. The example below shows how to overlap two elements using negative margins.

    ```css
    .element1 {
        margin-bottom: -20px;
    }
    .element2 {
        margin-top: -20px;
    }
    ```

-   <b> Multiple Classes :</b>
    An element can have multiple classes. Multiple classes can be added to an element by separating them with a space. The example below shows how to add two classes to a paragraph element.

    ```css
    .class1 {
        color: blue;
    }
    .class2 {
        font-size: 20px;
    }
    ```

    ```HTML
    <p class="class1 class2">This is a paragraph.</p>
    ```

-   <b> Color Models :</b> There are two main color models. The <i>additive color model (RGB)</i> and the <i>subtractive color model (CMYK)</i>. The RGB color model is used for digital displays, while the CMYK color model is used for printing.

-   <b> The CSS RGB function </b> is used to specify colors using the RGB color model. The RGB function takes three parameters: the amount of red, green, and blue in the color. The example below shows how to specify the color red using the RGB function.

    ```css
    p {
        color: rgb(255, 0, 0);
    }
    ```

[[ref/Properties]]

## Understanding Colors

Colors are an important aspect of web design. They can be used to create visual interest, establish a mood, and communicate information. To be able to use colors effectively in web design, it is important to understand the different color models and how to specify colors in CSS. Each color model has its own set of primary, secondary, and tertiary colors, as well as different ways to create new colors by combining them.

### RGB Color Model

The RGB color model is an additive color model in which red, green, and blue light are added together in various ways to reproduce a broad array of colors.

Primary colors in the RGB color model are red, green, and blue. They are represented in CSS using the following RGB functions:

-   Red: `rgb(255, 0, 0)`
-   Green: `rgb(0, 255, 0)`
-   Blue: `rgb(0, 0, 255)`

Secondary colors are cyan, magenta, and yellow. They are represented in CSS using the following RGB functions:

-   Cyan: `rgb(0, 255, 255)`
-   Magenta: `rgb(255, 0, 255)`
-   Yellow: `rgb(255, 255, 0)`

The tertiary are orange, chartreuse, spring green, azure, violet, and rose. They are represented in CSS using the following RGB functions:

-   Orange: `rgb(255, 165, 0)`
-   Chartreuse: `rgb(127, 255, 0)`
-   Spring Green: `rgb(0, 255, 127)`
-   Azure: `rgb(0, 127, 255)`
-   Violet: `rgb(127, 0, 255)`
-   Rose: `rgb(255, 0, 127)`
-   And many more...

### HSL Color Model

The HSL color model is a cylindrical-coordinate representation of colors. It is based on the hue, saturation, and lightness of a color. The hue is the color type, the saturation is the intensity of the color, and the lightness is the brightness of the color. The HSL color model is represented in CSS using the following HSL functions:

-   Red: `hsl(0, 100%, 50%)`
-   Green: `hsl(120, 100%, 50%)`
-   Blue: `hsl(240, 100%, 50%)`
-   Cyan: `hsl(180, 100%, 50%)`
-   Magenta: `hsl(300, 100%, 50%)`
-   Yellow: `hsl(60, 100%, 50%)`
-   And many more...`

[[task/projects/Color-Palette]]

### The Hexadecimal Color System

The hexadecimal color system is a way of representing colors using a six-digit code. Each digit in the code represents a different color channel: red, green, and blue. The code is written as a hash symbol followed by six digits. For example, the color red is represented by `#FF0000`, where `FF` represents the red channel, `00` represents the green channel, and `00` represents the blue channel.

-   Red: `#FF0000`
-   Green: `#00FF00`
-   Blue: `#0000FF`
-   Cyan: `#00FFFF`
-   Magenta: `#FF00FF`
-   Yellow: `#FFFF00`
-   And many more...

## General CSS Property Rules, Tips and Tricks

-   When using the shorthand properties like `margin`, `padding`, `border`, `background`, etc., it is important to specify all the values in the correct order. The order of values for these properties is `top`, `right`, `bottom`, and `left`.

    ```css
    .element {
        margin: 10px 20px 30px 40px;
    }
    ```

-   When using the `border` property, you can specify the border width, style, and color in a single declaration. The order of values for the `border` property is `width`, `style`, and `color`.
    ```css
    .element {
        border: 1px solid black;
    }
    ```
-   The `unset` value is used to reset a property to its inherited value if it inherits from its parent, or to its initial value if it does not inherit from its parent.

    ```css
    .element {
        margin: unset;
    }
    ```

-   To ensure that a property is always applied to an element, use the `!important` keyword. The `!important` keyword overrides any other styles that are applied to the element.

    ```css
    .element {
        color: red !important;
    }
    ```