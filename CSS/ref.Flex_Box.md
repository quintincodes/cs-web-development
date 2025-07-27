
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Flex_Box
---

#reference #css

created: 1721486814958
updated: 1738275940417
---


<!--#region styles-->

<!--#endregion-->

# Flex Box

![Flexbox](vd9dc7wfk9471.png)

The Flex Box is a layout model that allows you to design a layout in a more efficient way. It is a one-dimensional layout model that allows you to align items in a row or a column. The content in the flex box are called flex items. The Flex Box model is very powerful and can be used to create complex layouts with ease. To use the flex box model, you need to set the display property of the container to flex. Here is an example of how to use the flex box model.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Flex Box Example</title>
        
    </head>
    <body>
        <div class="container">
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
        </div>
    </body>
</html>
```

Flex box has a main axis and a cross axis. The main axis is defined by the flex-direction property.

-   `row` (default): horizontal axis with flex items from left to right

-   `row-reverse`: horizontal axis with flex items from right to left
-   `column`: vertical axis with flex items from top to bottom
-   `column-reverse`: vertical axis with flex items from bottom to top

<b>Note :</b> <i>The axes and directions will be different depending on the text direction. The values shown are for a left-to-right text direction.</i>