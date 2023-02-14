# Lecture 03

## CSS Backgrounds

CSS background properties are used to add background effects for elements

## background-color
background-color property specifies the background color of an element

```css
body {
  background-color: lightblue;
}
```
Opacity 
opacity property specifies the opacity/transparency of an element
value from 0.0 - 1.0
```css
div {
  background-color: green;
  opacity: 0.3;
}
```
Note:
When using the opacity property to add transparency to the background of an element, all of its child elements inherit the same transparency. 

Transparency using RGBA
If you do not want to apply opacity to child elements, like in our example above, use RGBA color values. The following example sets the opacity for the background color and not the text:

```css
div {
  background: rgba(0, 128, 0, 0.3) /* Green background with 30% opacity */
}
```

## background-image
background-image property specifies an image to use as the background of an element.

By default, the image is repeated so it covers the entire element.
```css
body {
  background-image: url("paper.gif");
}
```

## background-repeat
the background-image property repeats an image both horizontally and vertically.

Some images should be repeated only horizontally or vertically, or they will look strange, like this:

Example
body {
  background-image: url("gradient_bg.png");
}
If the image above is repeated only horizontally (background-repeat: repeat-x;), the background will look better:

Example
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
}
Tip: To repeat an image vertically, set background-repeat: repeat-y;

CSS background-repeat: no-repeat
Showing the background image only once is also specified by the background-repeat property:

Example
Show the background image only once:

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
}
In the example above, the background image is placed in the same place as the text. We want to change the position of the image, so that it does not disturb the text too much.

CSS background-position
The background-position property is used to specify the position of the background image.

Example
Position the background image in the top-right corner: 

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}

## background-attachment
background-attachment property specifies whether the background image should scroll or be fixed (will not scroll with the rest of the page):

Example
Specify that the background image should be fixed:

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
Example
Specify that the background image should scroll with the rest of the page:

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: scroll;
}
## background-position

## background (shorthand property)
background - Shorthand property
To shorten the code, it is also possible to specify all the background properties in one single property. This is called a shorthand property.

Instead of writing:

body {
  background-color: #ffffff;
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
You can use the shorthand property background:

Example
Use the shorthand property to set the background properties in one declaration:

body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}
When using the shorthand property the order of the property values is:

background-color
background-image
background-repeat
background-attachment
background-position
It does not matter if one of the property values is missing, as long as the other ones are in this order. Note that we do not use the background-attachment property in the examples above, as it does not have a value.