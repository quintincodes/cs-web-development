
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Properties
---

#reference #css

created: 1719783656246
updated: 1736075451980
---




**CSS properties are used to specify the appearance of an element. Properties are <B>key-value</B> pairs that are separated by a colon. <i>The key is the property name,</i> and the <i>value is the property value.</i> The property name is followed by a colon, and the property value is followed by a semicolon. The property value can be a <b>single value</b> or a <b>list of values</b> separated by commas. The property value can also be a <b>function</b> that returns a value.**

[[dendron://HTML/ref/elements]]

## Categories of CSS Properties

### Inheritable Properties

These properties are inherited from the parent element. This means that the child element will inherit the value of the property from the parent element if the child element does not have a value for the property. Examples of inheritable properties include `color`, `font-family`, `font-size`, `font-style`, `font-weight`, `text-align`, `text-decoration`, `text-transform`, `line-height`, `letter-spacing`, `word-spacing`, `text-shadow`, `white-space`, `word-wrap`, `font-variant`, `font-stretch`, and `font-size-adjust`.

### Non-Inheritable Properties

These properties are not inherited from the parent element. This means that the child element will not inherit the value of the property from the parent element if the child element does not have a value for the property. Examples of non-inheritable properties include `width`, `height`, `margin`, `padding`, `border`, `border-radius`, `box-shadow`, `box-sizing`, `overflow`, `display`, `visibility`, `position`, `z-index`, `float`, `clear`, `clip-path`, `clip`, `transform`, `background`, `background-color`, `background-image`, `background-repeat`, `background-attachment`, `background-position`, `background-size`, `background-clip`, `background-origin`, `background-blend-mode`, `top`, `right`, `bottom`, `left`, `overflow-x`, `overflow-y`, `overflow-style`, `overflow-wrap`, `flex-direction`, `flex-wrap`, `flex-flow`, `justify-content`, `align-items`, `align-content`, `order`, `flex`, `align-self`, `flex-grow`, `flex-shrink`, `flex-basis`, `object-fit`, `grid-template-columns`, `grid-template-rows`, `grid-template-areas`, `grid-template`, `grid-column-gap`, `grid-row-gap`, `grid-gap`, `grid-column`, `grid-row`, `grid-area`, `justify-items`, `align-items`, `justify-content`, `align-content`, `place-items`, `place-content`, `grid-auto-columns`, `grid-auto-rows`, `grid-auto-flow`, `grid`, `grid-column-start`, `grid-column-end`, `grid-row-start`, `grid-row-end`, `grid-row-gap`, `grid-column-gap`, `grid-gap`, `grid-area`, `justify-self`, `align-self`, `transition`, `transition-property`, `transition-duration`, `transition-timing-function`, `transition-delay`, `animation`, `animation-name`, `animation-duration`, `animation-timing-function`, `animation-delay`, `animation-iteration-count`, `animation-direction`, `animation-fill-mode`, `animation-play-state`, `@keyframes`, `border-collapse`, `border-spacing`, `caption-side`, `empty-cells`, `table-layout`, `vertical-align`, `text-align`, `text-transform`, `list-style-type`, `list-style-image`, `list-style-position`, `list-style`, `cursor`, `opacity`, `margin-left`,etc.

## Common CSS Properties

### Text and Font Styles [[ref/Properties/Values#text-and-font-style]]

-   <b>color :</b> Specifies the color of the text.eg. `color: red;`

-   <b> font-family :</b> Specifies the font family of the text.eg. `font-family: 'Arial';` <b>NB:</b><i> Add a fallback font family in case the first font is not available.eg. `font-family: 'Arial', sans-serif;`</i>

-   <b> font-size :</b> Specifies the size of the text.eg. `font-size: 16px;`
-   <b> font-style :</b> Specifies the style of the font.eg. `font-style: italic;`
-   <b> font-weight :</b> Specifies the weight of the font.eg. `font-weight: bold;`
-   <b> text-align :</b> Specifies the alignment of the text.eg. `text-align: center;`
-   <b> text-decoration :</b> Specifies the decoration of the text.eg. `text-decoration: underline;`
-   <b> text-transform :</b> Specifies the transformation of the text.eg. `text-transform: uppercase;`
-   <b> line-height :</b> Specifies the height of the line.eg. `line-height: 1.5;`
-   <b> letter-spacing :</b> Specifies the spacing between the letters.eg. `letter-spacing: 2px;`
-   <b> word-spacing :</b> Specifies the spacing between the words.eg. `word-spacing: 2px;`
-   <b> text-shadow :</b> Specifies the shadow of the text.eg. `text-shadow: 2px 2px 2px black;`
-   <b> white-space :</b> Specifies the white space of the text.eg. `white-space: nowrap;`
-   <b> word-wrap :</b> Specifies the wrapping of the text.eg. `word-wrap: break-word;`
-   <b> font-variant :</b> Specifies the variant of the font.eg. `font-variant: small-caps;`
-   <b> font-stretch :</b> Specifies the stretch of the font.eg. `font-stretch: expanded;`
-   <b> font-size-adjust :</b> Specifies the adjustment of the font size.eg. `font-size-adjust: 0.5;`

---

### Box Model [[ref/Properties/Values#box-model]]

-   <b> width :</b> Specifies the width of the element.eg. `width: 100px;`

-   <b> height :</b> Specifies the height of the element.eg. `height: 100px; #REVISE
    > Sometimes the `vh` and `vw` units are used to set the height and width of an element to be a percentage of the viewport height and width.eg. `height: 100vh; width: 100vw;`. This means the element will take up the full height and width of the viewport. The `vmin` and `vmax` units are also used to set the height and width of an element to be a percentage of the viewport's smaller and larger dimension, respectively.eg. `height: 100vmin; width: 100vmax;`. This means the element will take up the full height of the viewport's smaller dimension and the full width of the viewport's larger dimension.
-   <b> margin :</b> Specifies the margin of the element.eg. `margin: 10px;`
-   <b> padding :</b> Specifies the padding of the element. eg. `padding: 10px;`
-   <b> border :</b> Specifies the border of the element.eg. `border: 1px solid black;`
-   <b> border-radius :</b> Specifies the radius of the border.eg. `border-radius: 10px;`
-   <b> box-shadow :</b> This property allows you to add one or more shadows to an element. Here is is a basic syntax: `box-shadow: offsetX offsetY color;`

    > Here's how the offsetX and offsetY values work:
    >
    > -   both offsetX and offsetY accept number values in px and other CSS units
    > -   a positive offsetX value moves the shadow right and a negative value moves it left
    > -   a positive offsetY value moves the shadow down and a negative value moves it up
    > -   if you want a value of zero (0) for any or both offsetX and offsetY, you don't need to add a unit. Every browser understands that zero means no change.

    > The height and width of the shadow is determined by the height and width of the element it's applied to. You can also use an optional `spreadRadius` value to spread out the reach of the shadow. A `blurRadius` value can also be added to blur the shadow. The syntax is as follows: `box-shadow: offsetX offsetY blurRadius spreadRadius color;`

-   <b> box-sizing :</b> This property specifies how the width and height of an element are calculated. The `content-box` value is the default value and includes only the content
-   . The `border-box` value includes the content, padding, and border.eg. `box-sizing: border-box;`

-   <b> overflow :</b> Specifies the overflow of the box.eg. `overflow: hidden;`
-   <b> display :</b> Specifies the display of the box.eg. `display: block;`
-   <b> visibility :</b> Specifies the visibility of the box.eg. `visibility: hidden;`
-   <b> position :</b> Specifies the position of the box.eg. `position: absolute;`
-   <b> z-index :</b> Specifies the z-index of the box. the z-index property specifies the stack order of an element. An element with greater stack order is always in front of an element with a lower stack order. Stack order is the order in which elements are stacked on top of each other.eg. `z-index: 1;`
-   <b> float :</b> Specifies the float of the box. This means that the element is removed from the normal flow of the document and placed to the left or right of the containing element.eg. `float: left;`
-   <b> clear :</b> This property specifies which sides of an element where other floating elements are not allowed.eg. `clear: both;`
-   <b> clip-path :</b> This property creates a clipping region that sets what part of an element should be shown.eg. `clip-path: circle(50%);`
-   <b> clip :</b> This property clips an absolutely positioned element.eg. `clip: rect(0px,60px,200px,0px);`
-   <b>transform :</b> This property allows you to rotate, scale, skew, or translate an element. Here is a basic syntax: `transform: rotate(30deg);`

    > The `rotate()` function rotates an element clockwise or counterclockwise by a specified number of degrees. The value of the angle can be positive or negative. The `scale()` function scales an element up or down by a specified factor. The value of the factor can be greater than 1 to scale up or less than 1 to scale down. The `skew()` function skews an element along the X and Y axes by a specified angle. The value of the angle can be positive or negative. The `translate()` function moves an element along the X and Y axes by a specified distance. The value of the distance can be positive or negative. The `matrix()` function combines all the 2D transform functions into one. The `matrix3d()` function combines all the 3D transform functions into one.

---

### Backgrounds [[ref/Properties/Values#Backgrounds]]

-   <b> background :</b> This property is a shorthand property for the `background-color`, `background-image`, `background-repeat`, `background-attachment`, `background-position`, and `background-size` properties.eg.
    ```css
    background: lightblue url('image.jpg') repeat-x right top fixed 100px 100px;
    ```
-   <b> background-color :</b> This property sets the background color of an element.eg. `background-color: lightblue;`

-   <b> background-image :</b> This property sets the background image of an element.eg. `background-image: url('image.jpg');`
-   <b> background-repeat :</b> This property sets how the background image is repeated.eg. `background-repeat: repeat-x;`
-   <b> background-position :</b> This property sets the starting position of the background image.eg. `background-position: right top;`
-   <b> background-attachment :</b> This property sets whether the background image is fixed or scrolls with the rest of the page.eg. `background-attachment: fixed;`
-   <b> background-size :</b> This property sets the size of the background image.eg. `background-size: 100px 100px;`
-   <b> background-clip :</b> This property specifies the painting area of the background.eg. `background-clip: padding-box;`
-   <b> background-origin :</b> This property specifies where the background image is positioned.eg. `background-origin: content-box;`
-   <b> background-blend-mode :</b> This property specifies the blending mode of the background image.eg. `background-blend-mode: multiply;`

---

### Positioning [[ref/Properties/Values#Positioning]]

-   <b> top :</b> This property specifies the top position of an element.eg. `top: 100px;`

-   <b> right :</b> This property specifies the right position of an element.eg. `right: 100px;`
-   <b> bottom :</b> This property specifies the bottom position of an element.eg. `bottom: 100px;`
-   <b> left :</b> This property specifies the left position of an element.eg. `left: 100px;`
-   <b> position :</b> This property specifies the type of positioning method used for an element.eg. `position: relative;`
-   <b> overflow-x :</b> This property specifies whether to clip the content, add a scroll bar, or display overflow content of an element.eg. `overflow-x: hidden;`
-   <b> overflow-y :</b> This property specifies whether to clip the content, add a scroll bar, or display overflow content of an element.eg. `overflow-y: scroll;`
-   <b> overflow-style :</b> This property specifies the style of the overflow.eg. `overflow-style: auto;`
-   <b> overflow-wrap :</b> This property specifies whether or not the browser should insert line breaks within words to prevent text from overflowing its content box.eg. `overflow-wrap: break-word;`

---

### Flexbox

-   <b> flex-direction :</b> This property specifies the direction of the flexible items.eg. `flex-direction: row;`

-   <b> flex-wrap :</b> This property specifies whether the flexible items should wrap or not.eg. `flex-wrap: wrap;`
-   <b> flex-flow :</b> This property is a shorthand property for the `flex-direction` and `flex-wrap` properties.eg. `flex-flow: row wrap;`
-   <b> justify-content :</b> This property aligns the flexible container's items when the items do not use all available space on the main-axis.eg. `justify-content: center;`
-   <b> align-items :</b> This property aligns the flexible container's items when the items do not use all available space on the cross-axis.eg. `align-items: center;`
-   <b> align-content :</b> This property aligns the flexible container's lines when there is extra space in the cross-axis.eg. `align-content: center;`
-   <b> order :</b> This property specifies the order of the flexible item.eg. `order: 2;`
-   <b> flex :</b> This property specifies the length of the item, relative to the rest of the flexible items inside the same container.eg. `flex: 2;`
-   <b> align-self :</b> This property specifies the alignment for the selected item inside the flexible container.eg. `align-self: center;`
-   <b> flex-grow :</b> This property specifies how much the item will grow relative to the rest of the flexible items inside the same container.eg. `flex-grow: 2;`
-   <b> flex-shrink :</b> This property specifies how the item will shrink relative to the rest of the flexible items inside the same container.eg. `flex-shrink: 2;`
-   <b> flex-basis :</b> This property specifies the initial length of the item.eg. `flex-basis: 100px;`
-   <b> object-fit :</b> This property specifies how the contents of a replaced element should be resized to fit its container.eg. `object-fit: cover;` <b>NB:</b><i> The `object-fit` property is used to specify how an image or video should be resized to fit its container. The `object-position` property is used to specify the alignment of the image or video within its container.</i>

---

### Grid

-   <b> grid-template-columns :</b> This property specifies the number (and the widths) of columns in a grid layout.eg. `grid-template-columns: 100px 100px 100px;`

-   <b> grid-template-rows :</b> This property specifies the number (and the heights) of rows in a grid layout.eg. `grid-template-rows: 100px 100px 100px;`
-   <b> grid-template-areas :</b> This property specifies the names of the grid areas.eg. `grid-template-areas: "header header header" "nav main main" "nav footer footer";`
-   <b> grid-template :</b> This property is a shorthand property for the `grid-template-rows`, `grid-template-columns`, and `grid-template-areas` properties.eg. `grid-template: 100px 100px / 100px 100px;`
-   <b> grid-column-gap :</b> This property specifies the size of the gap between the columns in a grid layout.eg. `grid-column-gap: 10px;`
-   <b> grid-row-gap :</b> This property specifies the size of the gap between the rows in a grid layout.eg. `grid-row-gap: 10px;`
-   <b> grid-gap :</b> This property is a shorthand property for the `grid-row-gap` and `grid-column-gap` properties.eg. `grid-gap: 10px 15px;`
-   <b> grid-column :</b> This property is a shorthand property for the `grid-column-start`, `grid-column-end`, `grid-row-start`, and `grid-row-end` properties.eg. `grid-column: 1 / 3;`
-   <b> grid-row :</b> This property is a shorthand property for the `grid-row-start` and `grid-row-end` properties.eg. `grid-row: 1 / 3;`
-   <b> grid-area :</b> This property is a shorthand property for the `grid-row-start`, `grid-column-start`, `grid-row-end`, and `grid-column-end` properties.eg. `grid-area: 1 / 1 / 3 / 3;`
-   <b> justify-items :</b> This property aligns the grid items in the grid along the inline (row) axis (as opposed to align-items which aligns the items across the block (column) axis).eg. `justify-items: center;`
-   <b> align-items :</b> This property aligns the grid items in the grid along the block (column) axis (as opposed to justify-items which aligns the items along the inline (row) axis).eg. `align-items: center;`
-   <b> justify-content :</b> This property aligns the grid along the inline (row) axis.eg. `justify-content: center;`
-   <b> align-content :</b> This property aligns the grid along the block (column) axis.eg. `align-content: center;`
-   <b> place-items :</b> This property is a shorthand property for the `align-items` and `justify-items` properties.eg. `place-items: center;`
-   <b> place-content :</b> This property is a shorthand property for the `align-content` and `justify-content` properties.eg. `place-content: center;`
-   <b> grid-auto-columns :</b> This property specifies the size of the columns in a grid layout.eg. `grid-auto-columns: 100px;`
-   <b> grid-auto-rows :</b> This property specifies the size of the rows in a grid layout.eg. `grid-auto-rows: 100px;`
-   <b> grid-auto-flow :</b> This property specifies how the auto-placement algorithm works, specifying exactly how auto-placed items get flowed into the grid.eg. `grid-auto-flow: row dense;`
-   <b> grid :</b> This property is a shorthand property for the `grid-template-rows`, `grid-template-columns`, `grid-template-areas`, `grid-auto-rows`, `grid-auto-columns`, and the `grid-auto-flow` properties.eg. `grid: 100px 100px / 100px 100px;`
-   <b> grid-column-start :</b> This property specifies on which column-line to start the item.eg. `grid-column-start: 2;`
-   <b> grid-column-end :</b> This property specifies on which column-line to end the item.eg. `grid-column-end: 4;`
-   <b> grid-row-start :</b> This property specifies on which row-line to start the item.eg. `grid-row-start: 2;`
-   <b> grid-row-end :</b> This property specifies on which row-line to end the item.eg. `grid-row-end: 4;`
-   <b> grid-row-gap :</b> This property specifies the size of the gap between the rows in a grid layout.eg. `grid-row-gap: 10px;`
-   <b> grid-column-gap :</b> This property specifies the size of the gap between the columns in a grid layout.eg. `grid-column-gap: 10px;`
-   <b> grid-gap :</b> This property is a shorthand property for the `grid-row-gap` and `grid-column-gap` properties.eg. `grid-gap: 10px 15px;`
-   <b> grid-area :</b> This property is a shorthand property for the `grid-row-start`, `grid-column-start`, `grid-row-end`, and `grid-column-end` properties.eg. `grid-area: 1 / 1 / 3 / 3;`
-   <b> justify-self :</b> This property aligns the grid item inside the grid area along the inline (row) axis.eg. `justify-self: center;`
-   <b> align-self :</b> This property aligns the grid item inside the grid area along the block (column) axis.eg. `align-self: center;`

---

### Transitions and Animations

-   <b> transition :</b> This property is a shorthand property for the `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay` properties.eg. `transition: width 2s;`
-   <b> transition-property :</b> This property specifies the name of the CSS property the transition effect is for.eg. `transition-property: width;`

-   <b> transition-duration :</b> This property specifies how many seconds or milliseconds a transition effect takes to complete.eg. `transition-duration: 2s;`
-   <b> transition-timing-function :</b> This property specifies the speed curve of the transition effect.eg. `transition-timing-function: linear;`
-   <b> transition-delay :</b> This property specifies when the transition effect will start.eg. `transition-delay: 1s;`
-   <b> animation :</b> This property is a shorthand property for the `animation-name`, `animation-duration`, `animation-timing-function`, `animation-delay`, `animation-iteration-count`, `animation-direction`, `animation-fill-mode`, and `animation-play-state` properties.eg. `animation: slide 3s ease 1s infinite alternate;`
-   <b> animation-name :</b> This property specifies the name of the `@keyframes` animation.eg. `animation-name: slide;`
-   <b> animation-duration :</b> This property specifies how many seconds or milliseconds an animation takes to complete.eg. `animation-duration: 3s;`
-   <b> animation-timing-function :</b> This property specifies the speed curve of the animation.eg. `animation-timing-function: ease;`
-   <b> animation-delay :</b> This property specifies when the animation will start.eg. `animation-delay: 1s;`
-   <b> animation-iteration-count :</b> This property specifies the number of times an animation should run.eg. `animation-iteration-count: infinite;`
-   <b> animation-direction :</b> This property specifies whether an animation should play in reverse direction or alternate cycles.eg. `animation-direction: alternate;`
-   <b> animation-fill-mode :</b> This property specifies what values are applied by the animation outside the time it is executing.eg. `animation-fill-mode: forwards;`
-   <b> animation-play-state :</b> This property specifies whether the animation is running or paused.eg. `animation-play-state: running;`
-   <b> @keyframes :</b> This rule specifies the animation code.eg. `@keyframes slide { from { left: 0px; } to { left: 100px; } }`

---

### Table Layout

-   <b> border-collapse :</b> This property specifies whether the table borders should be collapsed into a single border or separated.eg. `border-collapse: collapse;`

-   <b> border-spacing :</b> This property specifies the distance between the borders of adjacent cells.eg. `border-spacing: 10px;`
-   <b> caption-side :</b> This property specifies the placement of a table caption.eg. `caption-side: bottom;`
-   <b> empty-cells :</b> This property specifies whether or not to display borders and background on empty cells in a table.eg. `empty-cells: hide;`
-   <b> table-layout :</b> This property specifies the algorithm used to lay out the table cells, rows, and columns.eg. `table-layout: fixed;`
-   <b> vertical-align :</b> This property sets the vertical alignment of the content in a table cell.eg. `vertical-align: middle;`
-   <b> text-align :</b> This property sets the horizontal alignment of the content in a table cell.eg. `text-align: center;`
-   <b> text-transform :</b> This property transforms the text in a table cell.eg. `text-transform: uppercase;`

---

### Lists

-   <b> list-style-type :</b> This property specifies the type of list-item marker.eg. `list-style-type: circle;`

-   <b> list-style-image :</b> This property specifies an image as the list-item marker.eg. `list-style-image: url('image.jpg');`
-   <b> list-style-position :</b> This property specifies the position of the list-item marker.eg. `list-style-position: inside;`
-   <b> list-style :</b> This property is a shorthand property for the `list-style-type`, `list-style-position`, and `list-style-image` properties.eg. `list-style: circle inside url('image.jpg');`

---

### Miscellaneous

-   <b> cursor :</b> This property specifies the type of cursor to be displayed.eg. `cursor: pointer;`

-   <b> opacity :</b> This property sets the opacity level for an element.eg. `opacity: 0.5;`
-   <b> margin-left :</b> This property sets the left margin of an element.eg. `margin-left: 10px;`
-   <b> margin-right :</b> This property sets the right margin of an element.eg. `margin-right: 10px;`
-   <b> margin-top :</b> This property sets the top margin of an element.eg. `margin-top: 10px;`
-   <b> margin-bottom :</b> This property sets the bottom margin of an element.eg. `margin-bottom: 10px;`
-   <b>margin-auto:</b> This property sets the left and right margins of an element to auto, and the top and bottom margins to 0.eg. `margin: auto;`
-   <b> border-left-width :</b> This property sets the width of the left border.eg. `border-left-width: 10px;`
-   <b> border-right-width :</b> This property sets the width of the right border.eg. `border-right-width: 10px;`
-   <b> border-top-width :</b> This property sets the width of the top border.eg. `border-top-width: 10px;`
-   <b> border-bottom-width :</b> This property sets the width of the bottom border.eg. `border-bottom-width: 10px;`
-   <b> border-width :</b> This property is a shorthand property for the `border-top-width`, `border-right-width`, `border-bottom-width`, and `border-left-width` properties.eg. `border-width: 10px;`
-   <b> border-left-style :</b> This property sets the style of the left border.eg. `border-left-style: dotted;`
-   <b> border-right-style :</b> This property sets the style of the right border.eg. `border-right-style: dotted;`
-   <b> border-top-style :</b> This property sets the style of the top border.eg. `border-top-style: dotted;`
-   <b> border-bottom-style :</b> This property sets the style of the bottom border.eg. `border-bottom-style: dotted;`
-   <b> border-style :</b> This property is a shorthand property for the `border-top-style`, `border-right-style`, `border-bottom-style`, and `border-left-style` properties.eg. `border-style: dotted;`
-   <b> aspect-ratio :</b> This property sets the aspect ratio of an element.eg. `aspect-ratio: 16 / 9;`
-   <b> content :</b> This property is used with the `::before` and `::after` pseudo-elements to insert generated content.eg. `content: 'Hello';` <b>NB:</b><i> The `content` property is used with the `::before` and `::after` pseudo-elements to insert generated content. The `content` property can be used to insert text, images, counters, and other content before or after an element's content. The `content` property can also be used to insert an empty string to clear the content of an element.</i>