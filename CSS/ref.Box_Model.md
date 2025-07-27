
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Box_Model
---

#reference #css

created: 1721413191065
updated: 1738275940434
---


<!--#region styles-->

<!--#endregion-->

# Box Model

The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:

![CSS Box Model](<Box Modex.jpg>)

## Description

-   <b>Content</b> - The content of the box, where text and images appear. By default, the size of the content box is set using the `width` and `height` properties.

-   <b>Padding</b> - Clears an area around the content. The padding is transparent. The padding is affected by the background color of the box. The padding is used to create space around the content, inside of any defined borders.
-   <b>Border</b> - A border that goes around the padding and content. The border is affected by the background color of the box. The border is used to separate the padding and margin.
-   <b>Margin</b> - Clears an area outside the border. The margin is transparent. The margin does not have a background color, and is completely transparent.

<i>Example:</i>

```css
div {
    width: 300px;
    padding: 25px;
    border: 25px solid navy;
    margin: 25px;
}
```