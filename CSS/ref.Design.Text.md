
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Text
---

#reference #css

created: 1722421142690
updated: 1738275940425
---


<!--#region styles-->

<!--#endregion-->

# Text

### Making Text Visible To Only Screen Readers

```html
<p class="sr-only">This text is only visible to screen readers.</p>
```

```css
/* clip and rect are now deprecated */
.sr-only {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect(0, 0, 0, 0);
    white-space: nowrap;
    border: 0;
}
```

Here is a breakdown of the CSS properties used in the `.sr-only` class:

-   `position: absolute;`: This positions the element absolutely within its containing element.
-   `width: 1px;`: This sets the width of the element to 1 pixel.
-   `height: 1px;`: This sets the height of the element to 1 pixel.
-   `padding: 0;`: This removes any padding from the element.
-   `margin: -1px;`: This sets a negative margin to hide the element from view.
-   `overflow: hidden;`: This hides any content that overflows the element.
-   `clip: rect(0, 0, 0, 0);`: This clips the element to a 0x0 rectangle, effectively hiding it from view.
-   `white-space: nowrap;`: This prevents the element from wrapping onto multiple lines.
-   `border: 0;`: This removes any border from the element.

### Modern Way To Make Text Visible To Only Screen Readers

```html
<p class="visually-hidden">This text is only visible to screen readers.</p>
```

```css
.visually-hidden {
    clip: rect(0 0 0 0);
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap;
    width: 1px;
    border: 0;
}
```

Here is a breakdown of the CSS properties used in the `.visually-hidden` class:

-   `clip: rect(0 0 0 0);`: This clips the element to a 0x0 rectangle, effectively hiding it from view.
-   `clip-path: inset(50%);`: This clips the element to a 0x0 rectangle, effectively hiding it from view.
-   `height: 1px;`: This sets the height of the element to 1 pixel.
-   `overflow: hidden;`: This hides any content that overflows the element.
-   `position: absolute;`: This positions the element absolutely within its containing element.
-   `white-space: nowrap;`: This prevents the element from wrapping onto multiple lines.
-   `width: 1px;`: This sets the width of the element to 1 pixel.
-   `border: 0;`: This removes any border from the element.

<B>NB</B> **These classes are not used to hide only text, but any content that should be hidden from view but still accessible to screen readers.**