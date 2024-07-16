# Lecture - 03 (NESTED)

Sass Nested Rules and Properties
Sass Nested Rules
Sass lets you nest CSS selectors in the same way as HTML.

Nesting allows you to nest your CSS selectors in a way that follows the same visual hierarchy of your HTML. This makes your CSS more readable and maintainable. In SASS/SCSS, you can nest your CSS rules within one another to better represent the HTML structure.

Look at an example of some Sass code for a site's navigation:

Example
SCSS Syntax:

```css
.nav {
  background-color: $primary-color;

  .nav-item {
    color: $secondary-color;

    &:hover {
      color: darken($secondary-color, 10%);
    }
  }
}
```

Notice that in Sass, the ul, li, and a selectors are nested inside the nav selector.

While in CSS, the rules are defined one by one (not nested):

CSS Syntax:

```scss
.sidebar {
width: 300px;
float: left;

.widget {
margin-bottom: 20px;

    .widget-title {
      font-size: 1.5em;
      color: $primary-color;
    }
}
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

That's it for our second lecture on SASS/SCSS. Today, we covered how to use variables and nesting to make your CSS more manageable and readable. Do you have any questions? Feel free to ask! For further reading, check out the official SASS documentation and tutorials linked on the slide.

Resources:
SASS Official Documentation: https://sass-lang.com/documentation
SASS Variables Documentation: https://sass-lang.com/documentation/variables
SASS Nesting Documentation: https://sass-lang.com/documentation/style-rules/nesting