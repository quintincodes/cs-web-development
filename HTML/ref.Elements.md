
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: Elements
---

#reference #html

created: 1719555036117
updated: 1724443609710
---




## How HTML Elements Are Displayed

**HTML elements can either be <i>block-level elements</i> or <i>inline elements</i>. Block-level elements start on a new line and take up the full width available, while inline elements do not start on a new line and only take up as much width as necessary. Below is a table showing the inline and block-level elements in HTML**

| <b>Block-Level Elements</b> | <b>Inline Elements</b> | <b>Block-Level Elements</b> | <b>Inline Elements</b> |
| --------------------------- | ---------------------- | --------------------------- | ---------------------- |
| `<div>`                     | `<span>`               | `<figcaption>`              | `<button>`             |
| `<h1>` - `<h6>`             | `<a>`                  | `<time>`                    | `<textarea>`           |
| `<p>`                       | `<img>`                | `<progress>`                | `<select>`             |
| `<form>`                    | `<strong>`             | `<meter>`                   | `<option>`             |
| `<ul>`                      | `<em>`                 | `<details>`                 | `<label>`              |
| `<ol>`                      | `<i>`                  | `<summary>`                 | `<fieldset>`           |
| `<li>`                      | `<u>`                  | `<address>`                 | `<legend>`             |
| `<table>`                   | `<code>`               | `<blockquote>`              | `<b>`                  |
| `<tr>`                      | `<abbr>`               | `<pre>`                     | `<u>`                  |
| `<td>`                      | `<cite>`               | `<img>`                     | `<a>`                  |
| `<th>`                      | `<q>`                  | `<form>`                    | `<i>`                  |
| `<header>`                  | `<mark>`               | `<input>`                   | `<code>`               |
| `<footer>`                  | `<sub>`                | `<button>`                  | `<abbr>`               |
| `<nav>`                     | `<sup>`                | `<label>`                   | `<cite>`               |
| `<section>`                 | `<small>`              | `<select>`                  | `<q>`                  |
| `<article>`                 | `<br>`                 | `<article>`                 | `<br>`                 |
| `<aside>`                   | `<hr>`                 | `<figure>`                  | `<input>`              |

## Semantic HTML Elements

HTML5 introduced several new semantic elements. These elements tell the browser about the type of content they contain. This helps the browser to understand the structure of the document. Here are some of the most commonly used semantic elements:
[[ref/attributes]]

-   `<header>`:

Represents the header of a section or a page. It usually contains the logo, navigation links, and other elements.

```html
<header>
    <h1>My Website</h1>
    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>
</header>
```

-   `<nav>`:

Represents the navigation links of a page. It usually contains links to other pages or sections of the same page.

```html
<nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
</nav>
```

-   `<main>`:

Represents the main content of a page. It usually contains the main content of the page, such as articles, blog posts, or product listings.

```html
<main>
    <article>
        <h2>Article Title</h2>
        <p>Article content goes here...</p>
    </article>
</main>
```

-   `<article>`:

Represents an independent piece of content. It can be a blog post, a news article, a forum post, or any other piece of content.

```html
<article>
    <h2>Article Title</h2>
    <p>Article content goes here...</p>
</article>
```

-   `<section>`:

Represents a section of a document. It can contain multiple articles, blog posts, or other pieces of content.

```html
<section>
    <article>
        <h2>Article Title</h2>
        <p>Article content goes here...</p>
    </article>
</section>
```

-   `<aside>`:

Represents content that is tangentially related to the content around it. It can contain related links, advertisements, or other content.

```html
<aside>
    <h3>Related Links</h3>
    <ul>
        <li><a href="#">Link 1</a></li>
        <li><a href="#">Link 2</a></li>
        <li><a href="#">Link 3</a></li>
    </ul>
</aside>
```

-   `<footer>`:

Represents the footer of a section or a page. It usually contains copyright information, contact information, and other elements.

```html
<footer>
    <p>&copy; 2022 My Website</p>
    <p>
        Contact:
        <a
            href="mailto:
        [email protected]"
            >[email protected]</a
        >
    </p>
</footer>
```

-   `<figure>`:

Represents a figure or an illustration. It can contain an image, a video, a diagram, or any other type of content.

```html
<figure>
    <img src="image.jpg" alt="Image" />
    <figcaption>Image Caption</figcaption>
</figure>
```

-   `<figcaption>`:

Represents the caption of a figure. It is used to describe the content of the figure.

```html
<figure>
    <img src="image.jpg" alt="Image" />
    <figcaption>Image Caption</figcaption>
</figure>
```

-   `<time>`:

Represents a specific time or a range of time. It can be used to represent dates, times, or durations.

```html
<p>Published on <time datetime="2022-01-01">January 1, 2022</time></p>
```

-   `<mark>`:

Represents highlighted text. It is used to highlight a specific portion of text.

```html
<p>This is <mark>highlighted</mark> text.</p>
```

-   `<progress>`:

Represents the progress of a task. It can be used to show the progress of a file upload, a download, or any other task.

```html
<progress value="50" max="100"></progress>
```

-   `<meter>`:

Represents a scalar measurement within a known range. It can be used to represent the level of a battery, the temperature of a room, or any other scalar measurement.

```html
<meter value="50" min="0" max="100"></meter>
```

-   `<details>`:

Represents additional details that the user can view or hide. It can be used to show additional information about a topic.

```html
<details>
    <summary>Click to view details</summary>
    <p>Additional details go here...</p>
</details>
```

-   `<summary>`:

Represents a summary or a legend for a `<details>` element. It is used to provide a brief description of the content that can be viewed or hidden.

````html
<details>
    <summary>Click to view details</summary>
    <p>Additional details go here...</p>
</details>

- `
<address>
    `: Represents the contact information for the author of a document or an
    article. It can contain the author's name, email address, phone number, or
    any other contact information. ```html
    <address>
        <p>Written by John Doe</p>
        <p>
            Contact: <a href="mailto: [email protected]"> [email protected]</a>
        </p>
    </address>
</address>
````

-   `<blockquote>`:

Represents a block of quoted text. It is used to quote a passage from another source.

```html
<blockquote>
    <p>This is a quoted text.</p>
</blockquote>
```

-   `<q>`:

Represents a short inline quotation. It is used to quote a short passage from another source.

```html
<p>He said <q>This is a short quotation.</q></p>
```

-   `<cite>`:

Represents the title of a work. It is used to cite the title of a book, a movie, a song, or any other work.

```html
<p>
    The book <cite>The Great Gatsby</cite> was written by F. Scott Fitzgerald.
</p>
```

-   `<abbr>`:

Represents an abbreviation or an acronym. It is used to define an abbreviation or an acronym.

```html
<p>
    The <abbr title="World Health Organization">WHO</abbr> is a specialized
    agency of the United Nations.
</p>
```

-   `<role>`:

Represents the role of an element. It is used to define the role of an element in the document. It can take values such as `navigation`, `main`, `search`, `button`, `link`, `region` etc. The `region` attribute goes with the `label` attribute to specify what that region does. The `label` attribute is used to provide a text description of the region.

```html
<div role="navigation">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
</div>
```

## Non-Semantic HTML Elements

Non-semantic elements are those that do not convey any meaning to the browser. They are used to format the content of the page. Here are some of the most commonly used non-semantic elements:

-   `<div>`:

Represents a generic container for other elements. It is used to group elements together and apply styles to them.

```html
<div>
    <p>This is a paragraph inside a div element.</p>
</div>
```

-   `

Represents an inline container for text. It is used to apply styles to a specific portion of text.

```html
<p>This is a <span style="color: red;">red</span> word.</p>
```

-   `<br>`:

Represents a line break. It is used to break a line of text and start a new line.

```html
<p>This is the first line.<br />This is the second line.</p>
```

-   `<hr>`:

Represents a thematic break between paragraphs. It is used to separate content into different sections.

```html
<p>This is the first paragraph.</p>
<hr />
<p>This is the second paragraph.</p>
```

-   `<b>`:

Represents bold text. It is used to make text bold.

```html
<p>This is <b>bold</b> text.</p>
```

-   `<i>`:

Represents italic text. It is used to make text italic.

```html
<p>This is <i>italic</i> text.</p>
```

-   `<u>`:

Represents underlined text. It is used to underline text.

```html
<p>This is <u>underlined</u> text.</p>
```

-   `<s>`:

Represents strikethrough text. It is used to strike through text.

````html
- `<sup
    >`: Represents superscript text. It is used to display text above the
    baseline. ```html
    <p>This is <sup>superscript</sup> text.</p></sup
>
````

-   `<sub>`:

Represents subscript text. It is used to display text below the baseline.

```html
<p>This is <sub>subscript</sub> text.</p>
```

-   `<small>`:

Represents smaller text. It is used to make text smaller.

```html
<p>This is <small>small</small> text.</p>
```

-   `<strong>`:

Represents strong importance. It is used to indicate that the text has strong importance.

```html
<p>This is <strong>important</strong> text.</p>
```

-   `<em>`:

Represents emphasized text. It is used to indicate that the text is emphasized.

```html
<p>This is <em>emphasized</em> text.</p>
```

-   `<code>`:

Represents computer code. It is used to display computer code.

```html
<p>This is a <code>code</code> example.</p>
```

-   `<pre>`:

Represents preformatted text. It is used to display text exactly as it is written, including spaces and line breaks.

```html
<pre>
    This is
    preformatted
    text.
</pre>
```

-   `<img>`:

Represents an image. It is used to display an image on the page. The `alt` attribute is used to provide a text description of the image. The `src` attribute is used to specify the URL of the image. The `width` and `height` attributes can be used to specify the dimensions of the image. The `title` attribute can be used to provide a tooltip for the image.

```html
<img src="image.jpg" alt="Image" />
```

-   `<a>`:

Represents a hyperlink. It is used to create a link to another page or resource.

```html
<a href="https://www.example.com">Link</a>
```

-   `link`: Represents a link to an external resource. It is used to link to an external stylesheet, a favicon, or any other external resource.

```html
<link rel="stylesheet" href="styles.css" />
```

-   `<ul>`:

Represents an unordered list. It is used to create a list of items without any specific order.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

-   `<ol>`:

Represents an ordered list. It is used to create a list of items with a specific order.

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```

-   `<li>`:

Represents a list item. It is used to create an item in a list.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

-   `<table>`:

Represents a table. It is used to create a table with rows and columns.

```html
<table>
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
    </tr>
</table>
```

-   `<caption>`

Represents the caption of a table. It is used to describe the content of the table. The `caption` element should always be the first child of a table, but can be positioned with the caption-side CSS property.

```html
<table>
    <caption>
        Table Caption
    </caption>
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
    </tr>
</table>
```

-   `tbody`

Represents the body of a table. It is used to group the body content of a table. The `tbody` element should be used when the table has multiple sections, such as a header, body, and footer.

```html
<table>
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </tbody>
</table>
```

-   `<thead>`

Represents the header of a table. It is used to group the header content of a table. The `thead` element should be used when the table has multiple sections, such as a header, body, and footer.

```html
<table>
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </tbody>
</table>
```

-   `<tr>`

Represents a table row. It is used to create a row in a table.

```html

</tr>

<tr>
    <td>Data 1</td>
    <td>Data 2</td>
</tr>
```

-   `<th>`:

Represents a table header cell. It is used to create a header cell in a table.

```html
<tr>
    <th>Header 1</th>
    <th>Header 2</th>
</tr>
```

-   `<td>`:

Represents a table data cell. It is used to create a data cell in a table.

```html
<tr>
    <td>Data 1</td>
    <td>Data 2</td>
</tr>
```

-   `<form>`:

Represents a form. It is used to create a form for user input.

```html
<form action="/submit" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required />
    <button type="submit">Submit</button>
</form>
```

-   `<input>`:

Represents an input field. It is used to create a text input field, a checkbox, a radio button, or other types of input fields. [[ref/AI/copilot/input]] . There are various ways to include validation in the input field. These include:

> -   `required`: Specifies that the input field must be filled out before submitting the form.
>
> -   `pattern`: Specifies a regular expression pattern that the input field's value must match. eg. `pattern="[A-Za-z]{3}"` will only accept 3 alphabetic characters.
> -   `minlength`: Specifies the minimum number of characters required in the input field. eg. `minlength="3"` will require at least 3 characters.
> -   `maxlength`: Specifies the maximum number of characters allowed in the input field. eg. `maxlength="10"` will allow a maximum of 10 characters.
> -   `min`: Specifies the minimum value allowed in the input field. eg. `min="18"` will require a minimum value of 18.
> -   `max`: Specifies the maximum value allowed in the input field. eg. `max="100"` will allow a maximum value of 100.

```html
<input type="text" name="name" placeholder="Enter your name" required />
```

-   `<button>`:

Represents a button. It is used to create a button that can be clicked by the user.

```html
<button type="submit">Submit</button>
```

-   `<label>`:

Represents a label for an input field. It is used to describe the purpose of the input field.

```html
<label for="name">Name:</label>
<input type="text" id="name" name="name" required />
```

-   `<select>`:

Represents a dropdown list. It is used to create a dropdown list with multiple options. This element can have the following attributes: [[ref/Attributes]]

```html
<select name="color">
    <option value="red">Red</option>
    <option value="green">Green</option>
    <option value="blue">Blue</option>
</select>
```

-   `<option>`:

Represents an option in a dropdown list. It is used to create an option in a dropdown list.

```html
<select name="color">
    <option value="red">Red</option>
    <option value="green">Green</option>
    <option value="blue">Blue</option>
</select>
```

-   `<textarea>`:

Represents a multiline text input field. It is used to create a text input field that can contain multiple lines of text.

```html
<textarea name="message" placeholder="Enter your message" required></textarea>
```

-   `fieldset`: <b>this is semantic HTML</b>

Represents a group of related elements. It is used to group related elements together and apply styles to them.

```html
<fieldset>
    <legend>Personal Information</legend>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required />
</fieldset>
```

-   `<legend>`:

Represents a caption for a `fieldset` element. It is used to describe the purpose of the group of elements.

```HTML
<fieldset>
    <legend>Personal Information</legend>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required />
</fieldset>
```