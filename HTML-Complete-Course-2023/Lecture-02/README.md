# Lecture -02

## What is HTML ? and Why we use it 😎? ⬇️

> HTML is the standard markup language for creating Web pages".
> HTML describes the structure of a Web page with the series of elements

### Why we use these HTML elements what's theirR meaning? 👇

```html
<!DOCTYPE html> ➡️ declaration represents the document type, and helps browsers
to display web pages correctly. declaration is not case sensitive but it's Best
Practice.

<html>
  ➡️ element is the root element of an HTML page

  <head>
    ➡️ element contains meta information about the HTML page-

    <title>Lecture 02</title>
    ➡️ element specifies a title for the HTML page (which is shown in the
    browser's title bar or in the page's tab)

    <body>
      ➡️ element defines the document's body, and it is a container for all the
      visible contents, such as headings, paragraphs, images, hyperlinks,
      tables, lists, etc.
    </body>
  </head>
</html>
```

### What are HTML Elements ? 👇

> HTML element is everything from the start tag to the end tag:

```html
<tagname>Content goes here...</tagname> Start tag Element content End tag
```

_**Note**_:🪧

> Some HTML elements have no content (like the `<br>` element).

> These elements are called empty elements.
> 🪧 Empty elements do not have an end tag! `</end>`

#### Nested HTML Elements: ➡️ 👇

HTML elements can be nested (this means that elements can contain other elements).

> All HTML documents consist of nested HTML elements.

```html: ⬇️
<!DOCTYPE html>
Element is the root element
<html>
inside the <html> element there is a <body> element:
<body>
inside the <body> element there are two other elements: <h1> and <p>:
<h1>My First Heading</h1>
<p>
My first paragraph.
<p> hssoc
</p>

```
