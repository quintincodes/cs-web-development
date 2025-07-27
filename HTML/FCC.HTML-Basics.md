
> **Note**: This note contained custom CSS styling. Check the CSS snippets in Obsidian settings.

---
title: HTML-Basics
---

#freecodecamp #tutorial #html

created: 1719427578919
updated: 1724443609722
---




# HTML

**HTML stands for Hyper Text Markup Language. It is the standard markup language for creating Web pages. It describes the structure of a Web page and consists of a series of elements. HTML elements tell the browser how to display the content. HTML elements are represented by tags. <i>HTML tags</i> label pieces of content such as <i>"heading"</i>, <i>"paragraph"</i>, <i>"table"</i>, and so on. Browsers do not display the HTML tags, but use them to render the content of the page. Below is the industry standard html boilerplate.**

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta name="author" content="Author Name" />
        <meta name="description" content="A description of the page" />
        <meta name="keywords" content="keyword1, keyword2, keyword3" />
        <title>Page Title</title>
    </head>
    <body>
        <h1>This is a Heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

## Basic HTML

Below are some entry level basic <b>HTML</b> syntax features.

-   The `<!DOCTYPE html>` declaration

This is the first line of an <b>HTML</b> document. It tells the browser what version of <b>HTML</b> the page is written in. It is not a tag, it is an instruction to the web browser about what version of <b>HTML</b> the page is written in.

-   The `<html>` element

This element wraps all the content on the entire page and is sometimes known as the root element. It is also known as the document element.

-   The `<head>` element

This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes keywords, page descriptions, CSS style, character set declarations, and more.

-   The `<meta>` element

This element lives inside the head of your page and gives information about your page. This information isn't shown on the web page itself, but it is for the browser to read and understand. examples:

```html
<meta charset="UTF-8" />
<!-- sets the character set your document should use to UTF-8 -->
<meta name="author" content="Author Name" />
<!-- sets the author of the page -->
<meta name="description" content="A description of the page" />
<!-- sets the description of the page -->
<meta name="keywords" content="keyword1, keyword2, keyword3" />
<!-- sets the keywords for the page -->
```

-   The `<title>` element

This element sets the title of your page, which is the title that appears in the browser tab the page is loaded in.

-   The `<body>` element

This element contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, audio players, or more.

-   The `<h>` tag is used for headings.

There are 6 levels of importance, `<h1>` to `<h6>`. The first being the one with the highest importance.

-   The `p` tag is used for paragraphs.

-   End tags begin with a slash(/). eg. `</h2>`

-   Comments in <b>HTML</b> are written usinng `<!-- -->`
-   The `main` element

Used to define the most important part of an HTML document.

-   Nested elements

Should be placed two spaces to the right of the above element.

-   self-closing-tag

Elements with no closing tags eg. `img`, `br`, `hr`, `input`, `link`, `meta`, `area`, `base`, `col`, `command`, `embed`, `keygen`, `param`, `source`, `track`, `wbr`

[[ref/attributes]]

-   Anchor tag `<a>`

This is used to add links it goes with the `href` attribute. [[]]

-   The `<section>` element

This is a semantic element used to define sections in a document. It is used to group related content.

![[ref/Elements#semantic-html-elements]]

## The DOM (Document Object Model)

The DOM is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page. A Web page is a document. This document can be either displayed in the browser window or as the HTML source. But it is the same document in both cases. The Document Object Model (DOM) represents that same document so it can be manipulated. The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript. The DOM represents a document with a logical tree. Each branch of the tree ends in a node, and each node contains objects. DOM methods allow programmatic access to the tree; with them, you can change the document's structure, style, or content. Nodes can also have event handlers attached to them. Once an event is triggered, the event handlers get executed. The DOM is a W3C (World Wide Web Consortium) standard. The DOM defines a standard for accessing documents like HTML and XML. The W3C DOM standard is separated into 3 different parts:

-   Core DOM - standard model for all document types
-   XML DOM - standard model for XML documents
-   HTML DOM - standard model for HTML documents

### The HTML DOM

When a web page is loaded, the browser creates a Document Object Model of the page. The HTML DOM model is constructed as a tree of Objects:

![html DOM](pic_htmltree.gif)

With the object model, JavaScript gets all the power it needs to create dynamic HTML:

-   JavaScript can change all the HTML elements in the page
-   JavaScript can change all the HTML attributes in the page
-   JavaScript can change all the CSS styles in the page
-   JavaScript can remove existing HTML elements and attributes
-   JavaScript can add new HTML elements and attributes
-   JavaScript can react to all existing HTML events in the page
-   JavaScript can create new HTML events in the page

The HTML DOM is a standard object model and programming interface for HTML. It defines:

-   The HTML elements as objects
-   The properties of all HTML elements
-   The methods to access all HTML elements
-   The events for all HTML elements

In other words: The HTML DOM is a standard for how to get, change, add, or delete HTML elements.

## The `Referer` Header

The `Referer` header is an optional HTTP header that identifies the address of the webpage that linked to the resource being requested. By checking the referrer, the new webpage can see where the request originated. This information can be used for analytics, logging, or security purposes.

### Misspelling in HTTP Specification

The `Referer` header is misspelled as `Referer` in the HTTP specification.

### Usage

The `Referer` header is sent with the request to the new webpage. The new webpage can then use the information in the `Referer` header to determine how to respond to the request. For example:

-   The new webpage could use the `Referer` header to determine whether the request is coming from a trusted source.
-   It can track the source of the request for analytics purposes.

### When the `Referer` Header is Sent

The `Referer` header is not always sent with the request. Here are some scenarios:

-   **Not Sent**:

    -   If the user navigates directly to the new webpage by typing the URL into the address bar or by using a bookmark.

    -   If the user navigates to the new webpage from a secure webpage to an insecure webpage.
    -   If the user navigates to the new webpage from an insecure webpage to an insecure webpage.
    -   If the user navigates to the new webpage from a secure webpage to a secure webpage.

-   **Sent**:
    -   If the user navigates to the new webpage from an insecure webpage to a secure webpage.