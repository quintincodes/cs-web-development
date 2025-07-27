
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Colors
---

#reference #css

created: 1720306471108
updated: 1724443609685
---




## ADDING FLAT COLORS IN CSS

This can be done using the rgb function, hsl function, or hexadecimal notation as a value for the color property.

![[FCC/CSS-Basics#the-hexadecimal-color-system]]
![[FCC/CSS-Basics#RGB-Color-Model]]
![[FCC/CSS-Basics#HSL-Color-Model]]

## ADDING COLOR TRANSITIONS/GRADIENTS

This can be done using the linear-gradient function as a value for the background property. The linear-gradient function actually creates image element, and is usually paired with the background property which can accept an image as a value. The syntax for the linear-gradient function is as follows:

```css
background: linear-gradient(direction, color1, color2, ...);
```

where direction is the <i>angle of the gradient</i>, and color1, color2, ... are the <i>colors to be used in the gradient</i>. The direction can be specified in degrees, gradients, or to the side of the element.The colors can be specified using the rgb, hsl, or hexadecimal notation. eg:

```css
/*The gradient will be from red to blue. The 90deg sets the direction of the gradient to 90 degrees clockwise from the top of the element.*/
background: linear-gradient(90deg, red, blue);
```

The gradient direction can be specified in:

1. <b>Degrees:</b> Specifies the angle from the horizontal, where 0 degrees creates a left-to-right gradient, and angles increase clockwise. eg:

    ```css
    /* 90 degrees creates a bottom-to-top gradient */
    background: linear-gradient(90deg, color1, color2);
    ```

2. <b> Keywords:</b> Specifies the direction of the gradient. The keywords are <i>to top</i>, <i>to right</i>, <i>to bottom</i>, and <i>to left</i>. eg:

    ```css
    /* to right creates a left-to-right gradient */
    background: linear-gradient(to right, color1, color2);
    ```

A color stop can be added to the gradient by specifying the position of the color stop after the color. A color stop is a point in the gradient where the color changes. eg:

```css
/*The gradient will be from red to blue. The 90deg sets the direction of the gradient to 90 degrees clockwise from the top of the element. The color stop is at 50% of the gradient.*/
background: linear-gradient(90deg, red, blue 50%);
```

<b>NB:</b> #IMPORTANT

-   The linear-gradient function automatically arranges the colors even if the color stops are not specified.

-   The color stops are specified in percentages, and the percentage is relative to the size of the element.
-   The color stops can be specified in pixels, but this is not recommended as it is not responsive.
-   The gradient direction is set to <b>180deg</b> by default.
-   For more <b>abrupt color changes</b>, Use this syntax:
    ```CSS
    linear-gradient(
        var(--first-color) 0%,
        var(--first-color) 40%,
        var(--second-color) 40%,
        var(--second-color) 80%,
    );
    ```