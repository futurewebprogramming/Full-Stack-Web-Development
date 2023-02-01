# Lecture - 04

## What are HTML Attributes?

**HTML** _Attributes_ provide additional information about HTML elements.

Attributes are always specified in the **Start Tag**.

_**For Example**_

**_Style Attribute_**

> The style attribute is used to add styles to an element, such as color, font, size, and more.

```Javascript
<h2 style="color: black">Lecture  -04</h2>
```

**_Lang Attribute_**

> to declare the language of the Web page. This is meant to assist search engines and browsers.

```js
<html lang="en">
```

**_Title Attribute_**

> The title attribute defines some extra information about an element.

```js
<p title="I am Title">Hover</p>
```

<p
title="I am Title">Hover me</p>

_Single or Double Quotes?_

> In some situations, when the attribute value itself contains double quotes, it is necessary to use single quotes:

```html
' I am Inside Single Qoute' " I am Inside Double Qoute "
```

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

_**Link Element**_

> A Tag is used for attach any link any external or internal soruce.

```js
<a href="https://www.youtube.com/@futureprogramming/">Future Programming</a>
```

<a
href="https://www.youtube.com/@futureprogramming/" title="Future Programming">Future Programming</a>

_**Href Attribute**_

> Specifies the URL of the page the link goes to
