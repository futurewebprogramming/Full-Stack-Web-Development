# Lecture 10;

### HTML Lists


with HTML lists we can group a set of related items in lists.

### Unordered  List

unordered list starts with `<ul>` tag. Each list item starts with the `<li>` tag.

>list items will be marked with bullets `small black circles`.
```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

### List Item Marker
CSS `list-style-type` property is used to define style of list item marker

`disc` Sets list item marker to a bullet by default

`circle`    Sets the list item marker to a circle

`square`	Sets the list item marker to a square

`none`	list items will not be marked

### Nested Unorderd Lists

```html
<ul>
  <li>HTML</li>
  <li>JavaScript
    <ul>
      <li>React JS</li>
      <li>Vue JS</li>
    </ul>
  </li>
  <li>CSS</li>
</ul>

```

<ul>
  <li>HTML</li>
  <li>JavaScript
    <ul>
      <li>React JS</li>
      <li>Vue JS</li>
    </ul>
  </li>
  <li>CSS</li>
</ul>

### Orderd List

ordered list starts with `<ol>` tag. Each list item starts with the `<li>` tag.

>list items will be marked with _**numbers**_ .

```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>

# Type Attribute

>type attribute of the `<ol>` tag, defines the `type` of the `list item` marker

`type="1"`	list items will be numbered with numbers (default)

`type="A"`	list items will be numbered with uppercase letters

`type="a"`	list items will be numbered with lowercase letters

`type="I"`	list items will be numbered with uppercase roman numbers

`type="i"`	list items will be numbered with lowercase roman numbers

```html
<ol type="A">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```
<ol type="i">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>

### Control List Counting

By default, ordered list will start counting from 1. If you want to start counting from a specified number, you can use the start attribute

```html
<ol start="70">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```
<ol type="i">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>

### Description Lists 

Description list is a `list of terms`, with a Description of each term

`<dl>` tag defines the `description list`,

`<dt>` tag defines the `term (name)`, 

`<dd>` tag `describes each term`


```html
<dl>
  <dt>HTML</dt>
  <dd>Hyper Text Markup Language is used for to make a web page structure</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheet is used to design a Web Page.</dd>
</dl>
```

<dl>
  <dt>HTML</dt>
  <dd>Hyper Text Markup Language is used for to make a web page structure</dd>
  </dl>

  <dl>
  <dt>CSS</dt>
  <dd>Cascading Style Sheet is used to design a Web Page.</dd>
</dl>

