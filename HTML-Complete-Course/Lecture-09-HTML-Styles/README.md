# Lecture -09

## HTML Styles and How to write inline and Internal styles in html


> HTML style attribute is used to add styles to an element.


Now let's see how many ways to add styles to an HTML Element. 

We will also cover this in CSS Module,


In line CSS. 

using inline css style to HTML element, we pass style attribute. 

```html
<tagname style="property:value;"></tagname>
```

> property is a CSS property. value is a CSS value.

No of Properties we can use in style attribute, some we will cover and more u know will cover in our Beloved CSS Module ❤️
### Background Color

<p
style="background-color:blue; padding:10px;
">
I am a paragraph.
</p>

> CSS background-color property defines the background color for HTML element.

### Text Color

> CSS color property defines the text color for element

<p
style="color:yellow"
>
  I am a Yellow Color Text paragraph.
</p>

### Fonts

> CSS font-family property defines the font to be used for element

<p
  style="font-size:20px; font-family:verdana; color:blue"
>
  I am a paragraph.
</p>

### Text Alignment

> CSS text-align property defines the horizontal text alignment HTML element

<p
  style="font-size:20px; font-family:verdana; color:blue; background-color:powderblue; text-align:center"
>
I am a Center Aligned paragraph
</p>


### Internal CSS 

Now there is another way to Add Style in Our HTML Document. 


Now we have to add our `<style>` tag in head tag 

and then we have to select our HTML element by tag Name , our By class or id, 

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Lecture -09</title>
    <style>
        h1{
          background-color: yellow;
        }
    </style>
</head>

<body>
    <h1>Lecture -9</h1>

</body>

</html>
```

<!DOCTYPE html>
<html lang="en">

<head>
    <title>Lecture -09</title>
    <style>
        h2{
          background-color: blue;
          padding: 12px;
        }
    </style>
</head>

<body>
    <h2>Lecture -9</h2>

</body>

</html>