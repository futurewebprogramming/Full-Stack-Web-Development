# Lecture - 03 (NESTED)

Sass Nested Rules and Properties
Sass Nested Rules
Sass lets you nest CSS selectors in the same way as HTML.

Look at an example of some Sass code for a site's navigation:

Example
SCSS Syntax:

```scss

nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }
  li {
    display: inline-block;
  }
  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}

```

Notice that in Sass, the ul, li, and a selectors are nested inside the nav selector.

While in CSS, the rules are defined one by one (not nested):

CSS Syntax:

```scss
nav ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
nav li {
  display: inline-block;
}
nav a {
  display: block;
  padding: 6px 12px;
  text-decoration: none;
}
```

Because you can nest properties in Sass, it is cleaner and easier to read than standard CSS.

Sass Nested Properties
Many CSS properties have the same prefix, like font-family, font-size and font-weight or text-align, text-transform and text-overflow.

With Sass you can write them as nested properties:

Example
SCSS Syntax:

```scss
font: {
  family: Helvetica, sans-serif;
  size: 18px;
  weight: bold;
}

text: {
  align: center;
  transform: lowercase;
  overflow: hidden;
}
```

The Sass transpiler will convert the above to normal CSS:

CSS Output:

```scss
font-family: Helvetica, sans-serif;
font-size: 18px;
font-weight: bold;

text-align: center;
text-transform: lowercase;
text-overflow: hidden;
```
