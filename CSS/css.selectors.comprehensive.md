# CSS Selectors Complete Reference

#css #web-development #selectors #styling #frontend

created: 1723292400000
updated: 1723292400000

---

## Overview

CSS selectors are patterns used to select and style HTML elements. Understanding selectors is fundamental to effective CSS styling.

## Basic Selectors

### Universal Selector

Selects all elements on the page.

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

### Type Selector (Element Selector)

Selects all elements of a specific type.

```css
h1 {
  color: blue;
  font-size: 2rem;
}

p {
  line-height: 1.6;
  margin-bottom: 1rem;
}

div {
  background-color: lightgray;
}
```

### Class Selector

Selects elements with a specific class attribute.

```css
.container {
  max-width: 1200px;
  margin: 0 auto;
}

.btn {
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.text-center {
  text-align: center;
}
```

```html
<div class="container">
  <button class="btn">Click me</button>
  <p class="text-center">Centered text</p>
</div>
```

### ID Selector

Selects an element with a specific ID attribute.

```css
#header {
  background-color: navy;
  color: white;
  padding: 20px;
}

#navigation {
  position: fixed;
  top: 0;
  width: 100%;
}

#footer {
  background-color: #333;
  color: white;
  text-align: center;
  padding: 20px;
}
```

```html
<header id="header">Main Header</header>
<nav id="navigation">Navigation</nav>
<footer id="footer">Footer Content</footer>
```

## Combinator Selectors

### Descendant Selector (Space)

Selects elements that are descendants of another element.

```css
/* All p elements inside div elements */
div p {
  color: red;
}

/* All links inside navigation */
nav a {
  text-decoration: none;
  color: white;
}

/* All list items inside unordered lists */
ul li {
  list-style-type: none;
  padding: 5px 0;
}
```

```html
<div>
  <p>This will be red</p>
  <section>
    <p>This will also be red</p>
  </section>
</div>
```

### Child Selector (>)

Selects direct children only.

```css
/* Only direct p children of div */
div > p {
  font-weight: bold;
}

/* Direct list items of navigation ul */
nav > ul > li {
  display: inline-block;
  margin: 0 10px;
}
```

```html
<div>
  <p>Direct child - will be bold</p>
  <section>
    <p>Not direct child - won't be bold</p>
  </section>
</div>
```

### Adjacent Sibling Selector (+)

Selects the immediately following sibling.

```css
/* P element immediately after h2 */
h2 + p {
  margin-top: 0;
  font-weight: bold;
}

/* Image immediately after paragraph */
p + img {
  margin-top: 20px;
}
```

```html
<h2>Heading</h2>
<p>This paragraph will have no top margin and be bold</p>
<p>This paragraph is normal</p>
```

### General Sibling Selector (~)

Selects all following siblings.

```css
/* All p elements that follow h2 */
h2 ~ p {
  color: gray;
}

/* All images after first paragraph */
p ~ img {
  border: 2px solid #ddd;
}
```

## Attribute Selectors

### Basic Attribute Selectors

```css
/* Elements with title attribute */
[title] {
  border-bottom: 1px dotted;
}

/* Links with target attribute */
a[target] {
  background-color: yellow;
}

/* Input elements with required attribute */
input[required] {
  border: 2px solid red;
}
```

### Attribute Value Selectors

```css
/* Exact match */
input[type="text"] {
  padding: 8px;
  border: 1px solid #ccc;
}

input[type="email"] {
  background-color: #f0f8ff;
}

/* Links to external sites */
a[href="https://example.com"]
{
  color: orange;
}
```

### Attribute Value Pattern Matching

```css
/* Starts with */
a[href^="https://"]
{
  background: url("secure-icon.png") no-repeat left center;
  padding-left: 20px;
}

/* Ends with */
a[href$=".pdf"] {
  background: url("pdf-icon.png") no-repeat left center;
  padding-left: 20px;
}

/* Contains */
img[alt*="logo"] {
  max-width: 200px;
}

/* Word match */
div[class~="highlight"] {
  background-color: yellow;
}

/* Language attribute starts with */
p[lang|="en"] {
  font-family: "Times New Roman", serif;
}
```

## Pseudo-Class Selectors

### Dynamic Pseudo-Classes

```css
/* Link states */
a:link {
  color: blue;
  text-decoration: none;
}

a:visited {
  color: purple;
}

a:hover {
  color: red;
  text-decoration: underline;
}

a:active {
  color: orange;
}

/* Button interactions */
button:hover {
  background-color: #0056b3;
  transform: translateY(-2px);
}

button:active {
  transform: translateY(0);
}

button:focus {
  outline: 2px solid #007bff;
  outline-offset: 2px;
}
```

### Structural Pseudo-Classes

```css
/* First and last children */
li:first-child {
  font-weight: bold;
  color: green;
}

li:last-child {
  border-bottom: none;
}

/* Nth child patterns */
tr:nth-child(even) {
  background-color: #f2f2f2;
}

tr:nth-child(odd) {
  background-color: white;
}

/* Every third element */
div:nth-child(3n) {
  background-color: lightblue;
}

/* First 3 elements */
p:nth-child(-n + 3) {
  font-size: 1.2rem;
}
```

### Form Pseudo-Classes

```css
/* Input states */
input:focus {
  border-color: #007bff;
  box-shadow: 0 0 0 2px rgba(0, 123, 255, 0.25);
}

input:valid {
  border-color: green;
}

input:invalid {
  border-color: red;
}

input:required {
  background-color: #fff5f5;
}

input:disabled {
  background-color: #f5f5f5;
  cursor: not-allowed;
}

input:checked + label {
  font-weight: bold;
  color: green;
}
```

## Pseudo-Element Selectors

### Content Pseudo-Elements

```css
/* Before and after */
.quote::before {
  content: "" ";
    font-size: 2em;
    color: #666;
}

.quote::after {
    content: " "";
  font-size: 2em;
  color: #666;
}

/* Add icons with content */
.email::before {
  content: "📧 ";
}

.phone::before {
  content: "📞 ";
}
```

### Text Pseudo-Elements

```css
/* First line styling */
p::first-line {
  font-weight: bold;
  color: #333;
}

/* First letter drop cap */
.article::first-letter {
  font-size: 3em;
  float: left;
  line-height: 1;
  margin-right: 5px;
  margin-top: 2px;
}

/* Selection styling */
::selection {
  background-color: #007bff;
  color: white;
}
```

## Advanced Selector Techniques

### Multiple Selectors

```css
/* Comma-separated selectors */
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Helvetica", sans-serif;
  margin-bottom: 0.5rem;
}

.btn,
.button,
input[type="submit"] {
  padding: 10px 15px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
```

### Chaining Selectors

```css
/* Element with multiple classes */
.btn.primary {
  background-color: #007bff;
  color: white;
}

.btn.secondary {
  background-color: #6c757d;
  color: white;
}

/* ID and class combination */
#header.sticky {
  position: fixed;
  top: 0;
  z-index: 1000;
}
```

### Complex Combinations

```css
/* Complex descendant patterns */
.sidebar ul li:last-child a:hover {
  background-color: #f8f9fa;
  border-radius: 4px;
}

/* Form styling combinations */
form .form-group input:not([type="submit"]):focus {
  border-color: #80bdff;
  box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
}
```

## Selector Specificity

Understanding CSS specificity hierarchy:

1. **Inline styles**: 1000 points
2. **IDs**: 100 points each
3. **Classes, attributes, pseudo-classes**: 10 points each
4. **Elements and pseudo-elements**: 1 point each

```css
/* Specificity: 1 (element) */
p {
  color: black;
}

/* Specificity: 10 (class) */
.text {
  color: blue;
}

/* Specificity: 100 (ID) */
#content {
  color: red;
}

/* Specificity: 111 (ID + class + element) */
#content .text p {
  color: green;
}
```

## Practical Examples

### Navigation Menu

```css
.nav {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav > li {
  position: relative;
}

.nav > li > a {
  display: block;
  padding: 15px 20px;
  text-decoration: none;
  color: #333;
  transition: background-color 0.3s;
}

.nav > li > a:hover {
  background-color: #f8f9fa;
}

.nav > li.active > a {
  background-color: #007bff;
  color: white;
}
```

### Card Component

```css
.card {
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.card:hover {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
  transform: translateY(-2px);
}

.card > .card-header {
  background-color: #f8f9fa;
  padding: 15px;
  border-bottom: 1px solid #ddd;
}

.card > .card-body {
  padding: 15px;
}

.card > .card-footer {
  background-color: #f8f9fa;
  padding: 10px 15px;
  border-top: 1px solid #ddd;
}
```

This comprehensive guide covers the essential CSS selectors needed for effective web styling and layout control.
