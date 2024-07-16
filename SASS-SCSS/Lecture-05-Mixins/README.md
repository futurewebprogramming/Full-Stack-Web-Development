
# Lecutre -05 Mixins

Sass `@mixin` and `@include`

## Sass Mixins

The @mixin directive lets you create CSS code that is to be reused throughout the website.

## Sass include

The @include directive is created to let you use (include) the mixin.

Defining a Mixin
A mixin is defined with the @mixin directive.

Sass @mixin Syntax:

```scss
@mixin name {
  property: value;
  property: value;
  ...
}
```

The following example creates a mixin named "important-text":

SCSS Syntax:

```scss
@mixin important-text {
  color: red;
  font-size: 25px;
  font-weight: bold;
  border: 1px solid blue;
}
```

Tip: A tip on hyphens and underscore in Sass: Hyphens and underscores are considered to be the same. This means that @mixin important-text { } and @mixin important_text { } are considered as the same mixin!

## Using a Mixin

The @include directive is used to include a mixin.

Sass @include mixin Syntax:

```scss
selector {
  @include mixin-name;
}
```

So, to include the important-text mixin created above:

SCSS Syntax:

```scss
.danger {
  @include important-text;
  background-color: green;
}
```

The Sass transpiler will convert the above to normal CSS:

CSS output:

```scss
.danger {
  color: red;
  font-size: 25px;
  font-weight: bold;
  border: 1px solid blue;
  background-color: green;
}
```

A mixin can also include other mixins:

SCSS Syntax:

```scss
@mixin special-text {
  @include important-text;
  @include link;
  @include special-border;
}
```

Passing Variables to a Mixin
Mixins accept arguments. This way you can pass variables to a mixin.

Here is how to define a mixin with arguments:

SCSS Syntax:

Define mixin with two arguments 

```scss
@mixin bordered($color, $width) {
  border: $width solid $color;
}

.myArticle {
  @include bordered(blue, 1px);  // Call mixin with two values
}

.myNotes {
  @include bordered(red, 2px); // Call mixin with two values
}
```

Notice that the arguments are set as variables and then used as the values (color and width) of the border property.

After compilation, the CSS will look like this:

CSS Output:

```scss
.myArticle {
  border: 1px solid blue;
}

.myNotes {
  border: 2px solid red;
}
```

Default Values for a Mixin
It is also possible to define default values for mixin variables:

SCSS Syntax:

```scss
@mixin bordered($color: blue, $width: 1px) {
  border: $width solid $color;
}
```

Then, you only need to specify the values that change when you include the mixin:

SCSS Syntax:

```scss
.myTips {
  @include bordered($color: orange);
}
```

Using a Mixin For Vendor Prefixes
Another good use of a mixin is for vendor prefixes.

Here is an example for transform:

SCSS Syntax:

```scss
@mixin transform($property) {
  -webkit-transform: $property;
  -ms-transform: $property;
  transform: $property;
}

.myBox {
  @include transform(rotate(20deg));
}
```

After compilation, the CSS will look like this:

CSS Output:

```scss
.myBox {
  -webkit-transform: rotate(20deg);
  -ms-transform: rotate(20deg);
  transform: rotate(20deg);
}
```
