# Lecture 1;

## CSS Introduction , Selectors, Syntax, & Comments.

## What is CSS?

CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.


### How To Add or include CSS in HTML

There are Three Ways to Insert CSS let's learn one by one.
### Inline CSS

An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element
```html
<h1 style="color:blue;text-align:center;">I am heading</h1>
```
### Internal CSS
An internal style sheet may be used if one single HTML page has a unique style.

internal style is defined inside the 
```css
<style> element, inside the head section.
```

### External CSS
With an external style sheet, you can change the look of an entire website by changing just one file!

External styles are defined within the `<link> `element, inside the `<head>` section of an HTML page

```html
<link rel="stylesheet" href="style.css">
```

### Highest Priority of Css

`1` - `Inline style` (inside an HTML element) have higher priority other than
`2`- `External and internal style` sheets (in the head section)
`3`- `Browser default`
### CSS Syntax

![CSS Example](https://www.w3schools.com/css/img_selector.gif "Good Example of CSS Syntax by W3 School")


### CSS Selector

CSS selectors are used to "find" (or select) the HTML elements you want to style

```css
    slector{
        property: value;
    }
```

### CSS Universal Selector

universal selector (*) selects all HTML elements on the page
```css
* {
  margin: 0;
  padding: 0;
}
```
### Simple selectors 
we select elements based on name, id, class

there are other ways as well but as we progressed in our course will learn. 

### Css id Selector

id selector uses the id attribute of an HTML element to select a specific element

To select an element with a specific id, write a hash `#idName`

```css
    #para{
        background-color: blue;
    }
```

### CSS class Selector

 class selector selects HTML elements with a specific class attribute

 To select elements with a specific class, write a `.classname`

```css
    .para{
        background-color: blue;
    }
```

we can also specify that only specific HTML elements should be affected by a class

```css
    p.para{
        background-color: blue;
    }
```

HTML elements can also have more than one class

```html
<p class="para main">I am Para.</p>
```


### CSS Grouping Selector

Sometime we want to style same styles on multiple elements so for that It will be better to group the selectors, to minimize the code, rather writing one by one.

```css
h1, h2, p {
  background-color: blue;
  color: white;
}
```

### CSS Comments

Comments are used to explain the code, and may help when you edit the source code at a later date.

Comments are ignored by browsers.
```css
/* This is a single-line comment */
p.para {
  color: black; /* text color set to black */
}
```

Comments can also span multiple lines: 

```css
/* This is
a multi-line
comment */
p.para {
  color: black; /* text color set to black */
}
```