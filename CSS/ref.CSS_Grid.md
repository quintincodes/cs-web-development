
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: CSS_Grid
---

#reference #css

created: 1724383574412
updated: 1738275940431
---


<!--#region styles-->

<!--#endregion-->

# CSS Grid

![CSS Grid](assets/images/CSS_Grid.jpg)

<small>Further Reading:</small>

-   <a href="https://css-tricks.com/snippets/css/complete-guide-grid/">CSS-Tricks: A Complete Guide to Grid</a>
-   <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout">MDN Web Docs: CSS Grid Layout</a>

## Introduction

CSS Grid is a powerful layout system available in CSS. It provides a two-dimensional grid-based layout system, optimized for building complex web layouts.

## Basic Concepts

-   <b>Grid Container</b>: The element on which `display: grid` is applied. It’s the direct parent of all the grid items.

-   <b>Grid Item</b>: The children of the grid container.
-   <b>Grid Lines</b>: The dividing lines that make up the structure of the grid, forming columns and rows.

### Creating a Grid

To create a grid, apply the `display: grid;` property to a container element.

```css
.container {
    display: grid;
}
```

### Defining Columns and Rows

To define the columns and rows of the grid, use the `grid-template-columns` and `grid-template-rows` properties.

```css
.container {
    display: grid;
    grid-template-columns: 100px 100px 100px;
    grid-template-rows: 100px 100px 100px;
}
```

### Placing Items on the Grid

To place items on the grid, use the `grid-column` and `grid-row` properties. You can specify the start and end positions of the item on the grid.

```css
.item {
    grid-column: 1 / 3; /* item spans from column line 1 to column line 3 */
    grid-row: 1 / 3; /* item spans from row line 1 to row line 3 */
}
```

### Grid Areas

You can also define named grid areas and place items within them. This means you can define areas of the grid and place items in those areas by referring to the area name.

```css
.container {
    display: grid;
    grid-template-areas:
        'header header header'
        'sidebar content content'
        'footer footer footer';
}

.item1 {
    grid-area: header;
}

.item2 {
    grid-area: sidebar;
}
```

### Responsive Design With CSS Grid

CSS Grid makes it easy to create responsive layouts. You can use media queries to change the layout of the grid based on the screen size.

```css
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}

@media screen and (max-width: 600px) {
    .container {
        grid-template-columns: 1fr;
    }
}
```

## Parent Properties & Values

-   <b>display</b>: Defines the element as a grid container and establishes a new grid formatting context for its contents. <b>Values:</b> `grid`, `inline-grid`.

-   <b>grid-template-columns</b>: Defines the columns of the grid. <b>Values:</b> `<track-size>`, `<line-name>`, `minmax()`, `repeat()`.
-   <b>grid-template-rows</b>: Defines the rows of the grid. <b>Values:</b> `<track-size>`, `<line-name>`, `minmax()`, `repeat()`.
-   <b>grid-template-areas</b>: Defines a grid template by referencing the names of the grid areas which are specified with the `grid-area` property. <b>Values:</b> `<string>`.

## The `fr` Unit

The `fr` unit represents a fraction of the available space in the grid container. It is used to distribute the available space in the grid container among the columns or rows.

```css
.container {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
}
```

#### Why Use The `fr` Unit ?

-   It makes it easy to create flexible layouts that adapt to the available space. For example, it helps avoid overflow or wrapping of content.

```css
.container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-column-gap: 10px;
}
```

In the above example, the `repeat()` function is used to create four columns with equal width, each taking up an equal fraction of the available space. Without using the `fr` unit, any other units will cause an overflow or wrapping of content if the available space is not enough.