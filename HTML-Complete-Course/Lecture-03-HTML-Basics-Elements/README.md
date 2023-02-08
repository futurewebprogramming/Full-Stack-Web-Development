# Lecture -03

In lecure 02 we have studied about introduction to html, what are elements and difference between elment and tags and structure of HTML elements. 🥰

In this Lecture we will study about: 👇
## Basic HTML Elements

Headings
Paragraphs
Links
Images 👇
br
hr &
Pre Tags

### What are Headings and Types of Headings in HTML ? 👇⬇️

> HTML headings are titles or subtitles that you want to display on a webpage.

Search engines use the headings to index the structure and content of your web pages.

> HTML headings are defined with the `<h1>` to `<h6>` tags.

```html
<h1>Heading 1 (Most Importan Heading).</h1>
<h2>Heading 2.</h2>
<h3>Heading 3.</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6 (least important heading).</h6>
```

<h1>Heading 1 (Most Importan Heading).</h1>
<h2>Heading 2.</h2>
<h3>Heading 3.</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6 (least important heading).</h6>

**_Note:_**

> Use HTML headings for headings only. Don't use headings to make text BIG or bold.

#### How to Write a Paragraph in HTML ? 👇⬇️

> A paragraph always starts on a new line, and is usually a block of text.

```html
<p>Defines a paragraph</p>
```

#### HTML Line Breaks

The HTML `<br>` element defines a line break.
Use `<br>` if you want a line break (a new line) without starting a new paragraph:

> `<br>` tag is an empty tag, which means that it has no end tag.

```html
<p>This is<br />a paragraph<br />with line breaks.</p>
```

<p>This is<br />a paragraph<br />with line breaks.</p>


## Image Element

```html
<img
  src="https://i.ytimg.com/vi/52klv1JkQF8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLD3LU1FTsVLpdmgxyUYaY-BPhXtrA"
/>
```

### Image Element Main Attributes

**_src_**

> to Provide Image Source.

```js
<img src="img1.png">
```

**_Alt Attribute_**

> If iamge not load properly due to any reason than alt Tag will show to user.

```js
<img src="img1.png" alt="I am image One">
```

<img
src="img1.png" alt="Image Not Loaded Properly, I am Alternative Text">

_**Width and Height Attributes**_

> To Specify image Width and Height we use widht and height Attribute

```js
<img src="img1.png" alt="I am image One" width="200px" height="200px">
```

<img
src="https://i.ytimg.com/vi/52klv1JkQF8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLD3LU1FTsVLpdmgxyUYaY-BPhXtrA" alt="I am image One" width="400px" height="200px" title="Full Stack Development Course">
_**Absolute URL**_

> Links to an external source that is hosted on another website

```html
<img src="https://i.ytimg.com/vi/52klv1JkQF8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLD3LU1FTsVLpdmgxyUYaY-BPhXtrA" alt="I am image One" width="200px" height="200px"
```

<img
src="https://i.ytimg.com/vi/52klv1JkQF8/hq720.jpg?sqp=-oaymwEcCOgCEMoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLD3LU1FTsVLpdmgxyUYaY-BPhXtrA" alt="I am image One" width="400px" height="200px">

_**Relative URL**_

> Links to internal source that is hosted within the website.

```js
<img src="img1.png" alt="I am image One" width="200px" height="200px">
```

### Link Element

> A Tag is used for attach any link any external or internal soruce.

```js
<a href="https://www.youtube.com/@futureprogramming/">Future Programming</a>
```

<a
href="https://www.youtube.com/@futureprogramming/" title="Future Programming">Future Programming</a>

_**Href Attribute**_

> Specifies the URL of the page the link goes to

_**Absolute URL**_

> Links to an external source that is hosted on another website

```html
<h2>Absolute URLs</h2>
<p><a href="https://www.github.com/">Github</a></p>
<p><a href="https://www.google.com/">Google</a></p>
```

_**Relative URL**_

> Links to internal source that is hosted within the website.


#### HTML Horizontal Rules 👇⬇️

---

The `<hr>` element is used to separate content (or define a change) in an HTML page:

> `<hr>` tag is an empty tag, which means that it has no end tag.

```html
<hr />
```

> `<hr />` element is used to separate content (or define a change) in an HTML page:

### HTML `<pre>` Element

> HTML `<pre>` element defines preformatted text.

Poem Project using `<pre>` Element

```html
<pre>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</pre>
```

<pre>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</pre>
