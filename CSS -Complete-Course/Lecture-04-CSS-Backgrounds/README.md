# Lecture 04

## CSS Backgrounds (Background-Color, Background Image, and it's properties)

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
!Important:
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

#### background-repeat

#### background-position

#### background-attachment

#### background-position

#### background (shorthand property)