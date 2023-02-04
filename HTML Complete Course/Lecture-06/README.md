# Lecture -06

## HTML `class` and `id` Attribute

HTML classes and IDs are used to select and style specific HTML elements with CSS also classes and IDs can be used to select and manipulate HTML elements in JavasScript.

### Classes?

Class is used to specify a `class attribute` to an HTML element. The value of the class attribute is the name of the class `For example:`

```html
<p class="highlight">This is a paragraph with a highlight class</p>
```

### Multiple Classes

Multiple elements can share the same class name

```html
<p class="highlight para">This is a paragraph with a highlight class</p>
```

>In CSS, classes are selected using a dot `(.)` before the class name.

For Example:

```css
.highlight {
  background-color: yellow;
}
```

### ID?

An ID is a `unique identifier` for a single element. An ID is defined by adding an id attribute to an HTML element.

#### ID Difference with Class

As we know id is uniuqe and we cannot use same id for other elements.

The value of the id attribute is the name of the ID, and each element can only have one `unique ID`.

 `For example:`

```html
<p id="first">This is a paragraph with a unique ID</p>
```

>In CSS, IDs are selected using a hash `(#)` before the ID name.

For example:

```css
#first {
  font-weight: bold;
}
```

### In JavaScript

Classes and IDs can be used to select and manipulate HTML elements.

#### Class

You can select elements with a specific class using the `document.getElementsByClassName()` method, which returns an array-like object of all elements with that class name. For example:

```js
var elements = document.getElementsByClassName("highlight");
```

#### ID

You can select a single element with a specific ID using the `document.getElementById()` method, which returns the first element with that ID. For example:

```js
var element = document.getElementById("first");

```
