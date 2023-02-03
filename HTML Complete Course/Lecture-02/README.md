# Lecture -02

## What is HTML ? Usage of Major HTML Elements 😎? ⬇️

> HTML is the standard markup language for creating Web pages".
> HTML describes the structure of a Web page with the series of elements

_Eample of HTML Websites:_

[WikiPedia](https://en.wikipedia.org/wiki/Main_Page "WikiPedia")

## What is an HTML Element?

> An HTML element is defined by a start tag, some content, and an end tag

_**For Example:**_

```js
<tagname> Content goes here... </tagname>
```

```js
<Start tag> Element content </End tag>
<h1> My First Heading </h1>
```

_**Note:**_

> Some HTML elements have no content

```js
(like the <br> element)
```

> These elements are called empty elements.

_**Empty Elements**_

> Empty elements do not have an end tag

_**Note:**_

The content inside the `<body>` section (the white area above) will be displayed in a browser.

The content inside the
`<title>`element will be shown in the browser's title bar or in the page's tab.

### Usage of Major HTML Elements Meaning 👇

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
