# Lecture -02

in Previous lecture we have installed our IDE and also installed some usefull Extensions and created our very first html file.

## Today

we will see how to use our extensions also we will learn about introudction of HTML and so on..

[![Full Stack Web Development](https://i.ytimg.com/vi/7GoKdXAwI9c/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLBvbwpml3MX1frFyxLFmHOBacVDmg "Introduction to HTML")](https://youtu.be/7GoKdXAwI9c)

## Introduction to HTML 😎? ⬇️

What is HTML and its importance

> HTML is the standard markup language for creating Web pages".
> HTML describes the structure of a Web page with the series of elements

_Eample of HTML Websites:_

[WikiPedia](https://en.wikipedia.org/wiki/Main_Page "WikiPedia")

## Difference B/W HTML elements and Tags?

Lot's of Confusion on the difference between HTML elements and Tags but i try to explain in simple way.

### HTML tags

> are just opening and closing tags without any content in between.

For Example

```html
<p></p>
are called HTML tags/elements
```

## HTML Element

> An HTML element is defined by a start tag, also have some content between, and an end tag

_**For Example:**_

```html
<h1>Heading 1</h1>
this is element now not just tags
```

is called HTML Element

> to more clarity jump around to this stack overflow debate
> [Difference B/W HTML Elements](https://stackoverflow.com/questions/8937384/what-is-the-difference-between-html-tags-and-elements)

_**Note:**_

> Some HTML Tags have no content

```html
(like the <br />
Tag)
```

> These tags are called empty tags/elements.

_**Empty tags / Elements**_

> Empty elements do not have an end tag

### Overview of HTML structure and syntax👇

```html
<!DOCTYPE html>
```

> `<!DOCTYPE html>` ➡️ declaration represents the document type, and helps browsers
> to display web pages correctly. declaration is not case sensitive but it's Best
> Practice.

```html
<html></html>
```

> ➡️ `<html>` element is the root element of an HTML page

```html
<head></head>
```

> `<head>`➡️ element contains meta information about the HTML page-

```html
<title>Lecture 02</title>
```

> `<title>`➡️ element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)

```html
<body></body>
```

> `<body>`➡️ element defines the document's body, and it is a _**container**_ for all the visible contents, such as ➡️ `<h1>headings</h1>` ,➡️ `<p>paragraphs </p>`, images `<img src="">`, `<a href="">hyperlinks</a>` ,`<table>tables</table>`, `<li>lists</li>`, etc.

#### Nested HTML Elements: ➡️ 👇

HTML elements can be nested (this means that elements can contain other elements).

> All HTML documents consist of nested HTML elements.

```html
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
</body>
</html>
```
