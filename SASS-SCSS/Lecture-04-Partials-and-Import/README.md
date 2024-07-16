# Lecture - 04

## Sass @import and Partials

Sass keeps the CSS code DRY (Don't Repeat Yourself). One way to write DRY code is to keep related code in separate files.

You can create small files with CSS snippets to include in other Sass files. Examples of such files can be: reset file, variables, colors, fonts, font-sizes, etc. 

### Sass Importing Files

Just like CSS, Sass also supports the @import directive.

The @import directive allows you to include the content of one file in another.

The CSS @import directive has a major drawback due to performance issues; it creates an extra HTTP request each time you call it. However, the Sass @import directive includes the file in the CSS; so no extra HTTP call is required at runtime!

### Sass Import Syntax:

@import filename;
Tip: You do not need to specify a file extension, Sass automatically assumes that you mean a .sass or .scss file. You can also import CSS files. The @import directive imports the file and any variables or mixins defined in the imported file can then be used in the main file.

You can import as many files as you need in the main file:

Example

```scss
@import "variables";
@import "colors";
@import "reset";
```

Let's look at an example: Let's assume we have a reset file called "reset.scss", that looks like this:

Example
SCSS Syntax (reset.scss):

```scss
html,
body,
ul,
ol {
  margin: 0;
  padding: 0;
}
```

and now we want to import the "reset.scss" file into another file called "standard.scss".

Here is how we do it: It is normal to add the @import directive at the top of a file; this way its content will have a global scope:

SCSS Syntax (standard.scss):

@import "reset";

```scss
body {
  font-family: Helvetica, sans-serif;
  font-size: 18px;
  color: red;
}
```

So, when the "standard.css" file is transpiled, the CSS will look like this:

CSS output:

```scss
html, body, ul, ol {
  margin: 0;
  padding: 0;
}

body {
  font-family: Helvetica, sans-serif;
  font-size: 18px;
  color: red;
}
```

### Sass Partials

By default, Sass transpiles all the .scss files directly. However, when you want to import a file, you do not need the file to be transpiled directly.

Sass has a mechanism for this: If you start the filename with an underscore, Sass will not transpile it. Files named this way are called partials in Sass.

So, a partial Sass file is named with a leading underscore:

### Sass Partial Syntax:

 _filename;
The following example shows a partial Sass file named "_colors.scss". (This file will not be transpiled directly to "colors.css"):

Example
"_colors.scss":

```scss
$myPink: #EE82EE;
$myBlue: #4169E1;
$myGreen: #8FBC8F;
```

Now, if you import the partial file, omit the underscore. Sass understands that it should import the file "_colors.scss":

Example
```@import "colors";```

```scss
body {
  font-family: Helvetica, sans-serif;
  font-size: 18px;
  color: $myBlue;
}
```
