
# Lecture -06 Sass @extend and Inheritance

## Sass @extend Directive

The `@extend` directive lets you share a set of CSS properties from one selector to another.

The `@extend` directive is useful if you have almost identically styled elements that only differ in some small details.

The following Sass example first creates a basic style for buttons (this style will be used for most buttons). Then, we create one style for a "Report" button and one style for a "Submit" button. Both "Report" and "Submit" button inherit all the CSS properties from the .button-basic class, through the @extend directive. In addition, they have their own colors defined:

SCSS Syntax:
```scss
.button-basic  {
border: none;
padding: 15px 30px;
text-align: center;
font-size: 16px;
cursor: pointer;
}

.button-report  {
@extend .button-basic;
background-color: red;
}

.button-submit  {
@extend .button-basic;
background-color: green;
color: white;
}
```

After compilation, the CSS will look like this:

CSS Output:
```scss
.button-basic, .button-report, .button-submit {
border: none;
padding: 15px 30px;
text-align: center;
font-size: 16px;
cursor: pointer;
}

.button-report  {
background-color: red;
}

.button-submit  {
background-color: green;
color: white;
}

```

By using the @extend directive, you do not need to specify several classes for an element in your HTML code, like this: <button class="button-basic button-report">Report this</button>. You just need to specify .button-report to get both sets of styles.

The @extend directive helps keep your Sass code very DRY.