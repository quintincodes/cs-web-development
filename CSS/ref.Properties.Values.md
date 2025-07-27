
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Values
---

#reference #css

created: 1720609849282
updated: 1724443609667
---




## Text and Font Style Values [[ref/Properties#text-and-font-styles]]

### Font-family

-

-   `font-family: Arial, sans-serif;` - The first font is used but its good practice to use a fallback font in case the first isn't available

### Font-size

-   `font-size: 16px;` - this is the default value in pixels.

-   ` font-size: 1em;` - `1em` is equal to `16px`. em is relative to the parent element's font-size

-   `font-size: 100%;` - Using percentages also sets the font-size relative to the parent element's font-size

### Font-style

-   `font-style: italic;`
-   `font-style: normal;` - This is the default value

-   `font-style: oblique;`

## Box Model [[ref/Properties#box-model]]

### Margin

-   `margin: 10px;` - This sets the margin on all sides of the element to `10px`

-   `margin: 10px 20px;` - This sets the top and bottom margin to `10px` and the left and right margin to `20px`
-   `margin: 10px 20px 30px;` - This sets the top margin to `10px`, the left and right margin to `20px` and the bottom margin to `30px`
-   `margin: 10px 20px 30px 40px;` - This sets the top margin to `10px`, the right margin to `20px`, the bottom margin to `30px` and the left margin to `40px`

### Padding

-   `padding: 10px;` - This sets the padding on all sides of the element to `10px`

-   `padding: 10px 20px;` - This sets the top and bottom padding to `10px` and the left and right padding to `20px`
-   `padding: 10px 20px 30px;` - This sets the top padding to `10px`, the left and right padding to `20px` and the bottom padding to `30px`
-   `padding: 10px 20px 30px 40px;` - This sets the top padding to `10px`, the right padding to `20px`, the bottom padding to `30px` and the left padding to `40px`

## Backgrounds [[ref/Properties#Backgrounds]]

### Background-color

-   `background-color: #f0f0f0;` - This uses the hexadecimal value for the color

-   `background-color: rgb(255, 0, 0);` - This uses the RGB value for the color
-   `background-color: rgba(255, 0, 0, 0.5);` - This uses the RGBA value for the color. The <i>alpha value</i> is used to set the transparency of the color
-   `background-color: hsl(120, 100%, 50%);` - This uses the HSL value for the color.
-   `background-color: hsla(120, 100%, 50%, 0.5);` - This uses the HSLA value for the color. The last value is the <i>alpha value</i>

### Background-image

-   `background-image: url('path/to/image.jpg');` - This sets the background image of the element to the image located at the specified path. The path can be a URL or a local file path.

-   `background-image: none;` - This removes the background image from the element
-   `background-image: linear-gradient(to right, red, blue);` - This creates a linear gradient background from red to blue
-   `background-image: radial-gradient(circle, red, blue);` - This creates a radial gradient background from red to blue
-   `background-image: repeating-linear-gradient(to right, red, blue 20%);` - This creates a repeating linear gradient background from red to blue with a 20% size
-   `background-image: repeating-radial-gradient(circle, red, blue 20%);` - This creates a repeating radial gradient background from red to blue with a 20% size

## Positioning [[ref/Properties#Positioning]]

-   `top: 10px;`
-   `right: 20px;`
-   `bottom: 30px;`
-   `left: 40px;`

### Position

-   `position: relative;` - This sets the element's position relative to its normal position. This means you can use the `top`, `right`, `bottom`, and `left` properties to move the element from its normal position.

-   `position: absolute;` - This sets the element's position relative to its parent element. If no parent element has a position set, it will be relative to the viewport (the browser window) instead of the parent element.
-   `position: fixed;` - This sets the element's position relative to the viewport (the browser window). The element will stay in the same place even when the page is scrolled. This is useful for elements like navigation bars.
-   `position: sticky;` - This sets the element's position relative to the viewport when scrolling up or down. The element will stick to the top of the viewport when it reaches a certain point. This is useful for elements like sticky headers.

### Z-index

-

-   `z-index: 10;` - This sets the element's stacking order. The higher the value, the closer the element is to the front. The default value is `0`

### Float

-   `float: right;` - This floats the element to the right. Other elements will wrap around it

-   `float: left;` - This floats the element to the left. Other elements will wrap around it. The default value is `none`
-

## Flexbox [[ref/Properties#Flexbox]]

### Flex-direction

-   `flex-direction: row;` - This sets the direction of the flex container's main axis to horizontal

-   `flex-direction: row-reverse;` - This sets the direction of the flex container's main axis to horizontal in reverse
-   `flex-direction: column;` - This sets the direction of the flex container's main axis to vertical
-   `flex-direction: column-reverse;` - This sets the direction of the flex container's main axis to vertical in reverse
-   `flex-wrap: nowrap;` - This sets the flex container to a single line. The default value is `nowrap`
-   `flex-wrap: wrap;` - This sets the flex container to multiple lines if needed.
-   `flex-wrap: wrap-reverse;` - This sets the flex container to multiple lines in reverse order if needed.
-   `justify-content: flex-start;` - This aligns the flex container's items to the start of the main axis. The default value is `flex-start`
-   `justify-content: flex-end;` - This aligns the flex container's items to the end of the main axis

### display

-   `display: flex;` - This sets the element as a flex container

-   `display: inline-flex;` - This sets the element as an inline flex container
-   `display: none;` - This hides the element. The element will not be displayed on the page
-   `display: block;` - This sets the element as a block-level element
-   `display: inline;` - This sets the element as an inline element
-   `display: inline-block;` - This sets the element as an inline block element
-   `display: grid;` - This sets the element as a grid container
-   `display: inline-grid;` - This sets the element as an inline grid container
-   `display: table;` - This sets the element as a table
-   `display: table-row;` - This sets the element as a table row
-   `display: table-cell;` - This sets the element as a table cell
-   `display: table-column;` - This sets the element as a table column
-   `display: table-row-group;` - This sets the element as a table row group
-   `display: table-column-group;` - This sets the element as a table column group
-   `display: table-header-group;` - This sets the element as a table header group
-   `display: table-footer-group;` - This sets the element as a table footer group
-   `display: table-caption;` - This sets the element as a table caption
-   `display: table-cell;` - This sets the element as a table cell

## Grid [[ref/Properties#Grid]]

### Grid-template-columns

-   `grid-template-columns: 100px 200px 300px;` - This sets the width of the columns in the grid to `100px`, `200px`, and `300px` respectively

-   `grid-template-columns: repeat(3, 1fr);` - This sets the width of the columns in the grid to `1fr` for 3 columns
-   `grid-template-columns: auto auto auto;` - This sets the width of the columns in the grid to `auto` for 3 columns
-   `grid-template-columns: 1fr 2fr 3fr;` - This sets the width of the columns in the grid to `1fr`, `2fr`, and `3fr` respectively
-   `grid-template-columns: 100px auto 200px;` - This sets the width of the columns in the grid to `100px`, `auto`, and `200px` respectively
-

## Transitions and Animations [[ref/Properties#Transitions-and-Animations]]

### Transition

-   `transition: all 0.3s ease-in-out;` - This sets the transition effect on all properties with a duration of `0.3s` and an easing function of `ease-in-out`

-   `transition: background-color 0.3s ease-in-out;` - This sets the transition effect on the `background-color` property with a duration of `0.3s` and an easing function of `ease-in-out`
-   `transition: color 0.3s ease-in-out, background-color 0.3s ease-in-out;` - This sets the transition effect on the `color` and `background-color` properties with a duration of `0.3s` and an easing function of `ease-in-out`
-   `transition: all 0.3s ease-in-out 0.1s;` - This sets the transition effect on all properties with a duration of `0.3s`, an easing function of `ease-in-out`, and a delay of `0.1s`
-

## Table Layout [[ref/Properties#Table-Layout]]

### Table-layout

-   `table-layout: auto;` - This is the default value. The table layout algorithm automatically calculates the column widths based on the content

-   `table-layout: fixed;` - The table layout algorithm uses the fixed layout. The column widths are set by the width of the first row of cells or the CSS width property
-

## Lists [[ref/Properties#Lists]]

### List-style-type

-   `list-style-type: disc;` - This sets the list item marker to a filled circle

-   `list-style-type: circle;` - This sets the list item marker to an empty circle
-   `list-style-type: square;` - This sets the list item marker to a square
-

## Miscellaneous [[ref/Properties#Miscellaneous]]

### Cursor

-   `cursor: pointer;` - This sets the cursor to a pointer (hand) when hovering over the element

-   `cursor: default;` - This sets the cursor to the default arrow when hovering over the element
-   `cursor: help;` - This sets the cursor to a help icon when hovering over the element
-   `cursor: not-allowed;` - This sets the cursor to a circle with a line through it when hovering over the element
-

<span>