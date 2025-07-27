
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Functions
---

#reference #css

created: 1720303139750
updated: 1724446735718
---




**CSS functions are used to manipulate the values of properties. They are used to perform operations on property values. They provide a way to perform complex operations on property values. A function is a keyword followed by a value and a closing parenthesis. The value is passed as an argument to the function. The function returns a value that is used to set the property value. Here are some of the functions used in CSS:** #REVISE

1. <b>The rgb() function :</b> The rgb() function is used to specify the color value using the RGB color model. It takes three arguments: red, green, and blue. The values range from 0 to 255 with 0 being the lowest value and 255 being the highest value. The syntax of the rgb() function is as follows:

    ```css
    color: rgb(255, 0, 0); /* red */
    color: rgb(0, 255, 0); /* green */
    color: rgb(0, 0, 255); /* blue */
    ```

2. <b>The rgba() function :</b> The rgba() function is used to specify the color value using the RGB color model with an alpha channel. <i>The alpha channel specifies the opacity of the color</i>. It takes four arguments: red, green, blue, and alpha. The alpha value ranges from 0 to 1 with 0 being fully transparent and 1 being fully opaque. The syntax of the rgba() function is as follows:

    ```css
    color: rgba(255, 0, 0, 0.5); /* red with 50% opacity */
    color: rgba(0, 255, 0, 0.5); /* green with 50% opacity */
    color: rgba(0, 0, 255, 0.5); /* blue with 50% opacity */
    ```

3. <b>The hsl() function :</b> The hsl() function is used to specify the color value using the HSL color model. It takes three arguments: hue, saturation, and lightness. The hue value ranges from 0 to 360, the saturation value ranges from 0% to 100%, and the lightness value ranges from 0% to 100%. The syntax of the hsl() function is as follows:

    ```css
    color: hsl(0, 100%, 50%); /* red */
    color: hsl(120, 100%, 50%); /* green */
    color: hsl(240, 100%, 50%); /* blue */
    ```

4. <b>The hsla() function :</b> The hsla() function is used to specify the color value using the HSL color model with an alpha channel. <i>The alpha channel specifies the opacity of the color</i>. It takes four arguments: hue, saturation, lightness, and alpha. The alpha value ranges from 0 to 1 with 0 being fully transparent and 1 being fully opaque. The syntax of the hsla() function is as follows:

    ```css
    color: hsla(0, 100%, 50%, 0.5); /* red with 50% opacity */
    color: hsla(120, 100%, 50%, 0.5); /* green with 50% opacity */
    color: hsla(240, 100%, 50%, 0.5); /* blue with 50% opacity */
    ```

5. <b>The url() function :</b> The url() function is used to specify the location of a resource, such as an image or a font file. It takes one argument: the URL of the resource. The syntax of the url() function is as follows:

    ```css
    background-image: url('image.jpg');
    font-family: url('font.woff');
    ```

6. <b>The calc() function :</b> The calc() function is used to perform mathematical calculations on property values. It takes one argument: a mathematical expression. The syntax of the calc() function is as follows:

    ```css
    width: calc(100% - 20px);
    height: calc(50vh - 10px);
    ```

7. <b>The var() function :</b> The var() function is used to specify a custom property value. It takes one argument: the name of the custom property. The syntax of the var() function is as follows:

    ```css
    color: var(--main-color);
    font-size: var(--font-size);
    ```

8. <b>The linear-gradient() function :</b> The linear-gradient() function is used to create a linear gradient background. It takes one or more arguments: the direction of the gradient and the color stops. The syntax of the linear-gradient() function is as follows:

    ```css
    background-image: linear-gradient(to right, red, blue);
    background-image: linear-gradient(45deg, red, blue);
    ```

9. <b>The radial-gradient() function :</b> The radial-gradient() function is used to create a radial gradient background. It takes one or more arguments: the shape of the gradient and the color stops. The syntax of the radial-gradient() function is as follows:

    ```css
    background-image: radial-gradient(circle, red, blue);
    background-image: radial-gradient(ellipse, red, blue);
    ```

10. <b>The repeating-linear-gradient() function :</b> The repeating-linear-gradient() function is used to create a repeating linear gradient background. It takes one or more arguments: the direction of the gradient, the color stops, and the size of the repeating pattern. The syntax of the repeating-linear-gradient() function is as follows:

    ```css
    background-image: repeating-linear-gradient(to right, red, blue 20px);
    background-image: repeating-linear-gradient(45deg, red, blue 20px);
    ```

11. <b>The repeating-radial-gradient() function :</b> The repeating-radial-gradient() function is used to create a repeating radial gradient background. It takes one or more arguments: the shape of the gradient, the color stops, and the size of the repeating pattern. The syntax of the repeating-radial-gradient() function is as follows:

    ```css
    background-image: repeating-radial-gradient(circle, red, blue 20px);
    background-image: repeating-radial-gradient(ellipse, red, blue 20px);
    ```

12. <b>The min() function :</b> The min() function is used to specify the minimum value of two or more property values. It takes two or more arguments: the property values. The syntax of the min() function is as follows:

    ```css
    width: min(100%, 200px);
    height: min(50vh, 100px);
    ```

13. <b>The max() function :</b> The max() function is used to specify the maximum value of two or more property values. It takes two or more arguments: the property values. The syntax of the max() function is as follows:

    ```css
    width: max(100%, 200px);
    height: max(50vh, 100px);
    ```

14. <b>The clamp() function :</b> The clamp() function is used to specify a value within a range of two other values. It takes three arguments: the minimum value, the preferred value, and the maximum value. The syntax of the clamp() function is as follows:

    ```css
    width: clamp(100px, 50%, 200px);
    height: clamp(50px, 25vh, 100px);
    ```

15. <b>The attr() function :</b> The attr() function is used to specify the value of an attribute. It takes one argument: the name of the attribute. The syntax of the attr() function is as follows:

    ```css
    content: attr(data-text);
    ```

16. <b>The counter() function :</b> The counter() function is used to insert the value of a counter. It takes one argument: the name of the counter. The syntax of the counter() function is as follows:

    ```css
    content: counter(section);
    ```

17. <b>The counters() function :</b> The counters() function is used to insert the values of multiple counters. It takes two arguments: the name of the counter and the separator. The syntax of the counters() function is as follows:

    ```css
    content: counters(section, '.');
    ```

18. <b>The toggle() function :</b> The toggle() function is used to toggle between two or more values. It takes two or more arguments: the values. The syntax of the toggle() function is as follows:

    ```css
    display: toggle(block, none);
    ```

19. <b>The cubic-bezier() function :</b> The cubic-bezier() function is used to specify a cubic Bézier curve for timing functions. It takes four arguments: the x and y coordinates of the first control point and the x and y coordinates of the second control point. The syntax of the cubic-bezier() function is as follows:

    ```css
    transition-timing-function: cubic-bezier(0.1, 0.7, 1, 0.1);
    ```

20. <b>The steps() function :</b> The steps() function is used to specify a step function for timing functions. It takes one or two arguments: the number of steps and the position of the end of the step. The syntax of the steps() function is as follows:

    ```css
    transition-timing-function: steps(4, end);
    ```

21. <b>The repeat() function :</b> The repeat() function is used to repeat a value a specified number of times. It takes two arguments: the value and the number of times to repeat it. The syntax of the repeat() function is as follows:

    ```css
    grid-template-columns: repeat(3, 1fr);
    ```

22. <b>The fit-content() function :</b> The fit-content() function is used to specify the size of a grid track based on its content. It takes one argument: the size of the track. The syntax of the fit-content() function is as follows:

    ```css
    grid-template-columns: fit-content(100px);
    ```

23. <b>The minmax() function :</b> The minmax() function is used to specify a size range for a grid track. It takes two arguments: the minimum size and the maximum size. The syntax of the minmax() function is as follows:

    ```css
    grid-template-columns: minmax(100px, 1fr);
    ```

24. <b>The blur() function :</b> The blur() function is used to apply a blur effect to an element. It takes one argument: the amount of blur. The syntax of the blur() function is as follows:

    ```css
    filter: blur(5px);
    ```

25. <b>The Rotate() function :</b> The rotate() function is used to rotate an element. It takes one argument: the angle of rotation. The syntax of the rotate() function is as follows:

    ```css
    transform: rotate(45deg);
    ```

26. <b>The scale() function :</b> The scale() function is used to scale an element. It takes one argument: the scale factor. The syntax of the scale() function is as follows:

    ```css
    transform: scale(1.5);
    ```

27. <b>The skew() function :</b> The skew() function is used to skew an element. It takes two arguments: the angles of skew in the x and y directions. The syntax of the skew() function is as follows:

    ```css
    transform: skew(30deg, 20deg);
    ```

28. <b>The translate() function :</b> The translate() function is used to move an element. It takes one argument: the distance to move the element. The syntax of the translate() function is as follows:

    ```css
    transform: translate(100px, 50px);
    ```

29. <b>The matrix() function :</b> The matrix() function is used to combine multiple transformations into a single matrix. It takes six arguments: the values of the matrix. The syntax of the matrix() function is as follows:

    ```css
    transform: matrix(1, 0, 0, 1, 100, 50);
    ```

30. <b>The matrix3d() function :</b> The matrix3d() function is used to combine multiple 3D transformations into a single matrix. It takes 16 arguments: the values of the matrix. The syntax of the matrix3d() function is as follows:

    ```css
    transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 100, 50, 0, 1);
    ```

31. <b>The minmax() function :</b> The minmax() function is used to specify a size range for a grid track. It takes two arguments: the minimum size and the maximum size. The syntax of the minmax() function is as follows:

    ```css
    grid-template-columns: minmax(100px, 1fr);
    ```