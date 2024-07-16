# Lecture - 02

## Sass Variables

Variables are a way to store information that you can re-use later.

With Sass, you can store information in variables, like:

```strings
numbers
colors
booleans
lists
nulls
```

Sass uses the `$ symbol`, followed by a name, to declare variables:

### Sass Variable Syntax

```$variablename: value;```
The following example declares 4 variables named myFont, myColor, myFontSize, and myWidth. After the variables are declared, you can use the variables wherever you want:

SCSS Syntax:

```scss
$myFont: Helvetica, sans-serif;
$myColor: red;
$myFontSize: 18px;
$myWidth: 680px;
```

```scss
body {
  font-family: $myFont;
  font-size: $myFontSize;
  color: $myColor;
}

#container {
  width: $myWidth;
}
```

So, when the Sass file is transpiled, it takes the variables (myFont, myColor, etc.) and outputs normal CSS with the variable values placed in the CSS, like this:

CSS Output:

```scss
body {
  font-family: Helvetica, sans-serif;
  font-size: 18px;
  color: red;
}

#container {
  width: 680px;
}
```

### Sass Variable Scope

Sass variables are only available at the level of nesting where they are defined.

Look at the following example:

SCSS Syntax:

```scss
$myColor: red;

h1 {
  $myColor: green;
  color: $myColor;
}

p {
  color: $myColor;
}
```

Will the color of the text inside a `<p>` tag be red or green? It will be red!

The other definition, `$myColor: green;` is inside the `<h1>` rule, and will only be available there!

So, the CSS output will be:

CSS Output:

```scss
h1 {
  color: green;
}

p {
  color: red;
}
```

Ok, that is the default behavior for variable scope.

### Using Sass !global

The default behavior for variable scope can be overridden by using the !global switch.

!global indicates that a variable is global, which means that it is accessible on all levels.

Look at the following example (same as above; but with !global added):

SCSS Syntax:

```scss
$myColor: red;

h1 {
  $myColor: green !global;
  color: $myColor;
}

p {
  color: $myColor;
}
```

Now the color of the text inside a `<p>` tag will be green!

So, the CSS output will be:

CSS Output:

```scss
h1 {
  color: green;
}

p {
  color: green;
}
```

Tip: Global variables should be defined outside any rules. It could be wise to define all global variables in its own file, named "_globals.scss", and include the file with the @include keyword