
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Pseudo_Elements
---

#reference #css

created: 1721493801212
updated: 1738275940410
---


<!--#region styles-->

<!--#endregion-->

# Pseudo Elements

### Definition

A pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element. They are typically used to style elements that are not directly accessible through the DOM (Document Object Model).

### Common Pseudo-elements

1. `::before`: Used to insert content before the content of an element.

2. `::after`: Used to insert content after the content of an element.
3. `::first-line`: Styles the first line of a block of text.
4. `::first-letter`: Styles the first letter of a block of text.
5. `::selection`: Styles the portion of text that a user has highlighted (selected).

### Syntax

```css
selector::pseudo-element {
    property: value;
}
```

### Example

```css
p::first-line {
    color: red;
    font-weight: bold;
}
```

In the example above, the `::first-line` pseudo-element is used to style the first line of all `<p>` elements in the document.