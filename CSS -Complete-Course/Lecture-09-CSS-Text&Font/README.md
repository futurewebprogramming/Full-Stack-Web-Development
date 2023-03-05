# Lecture -09

## CSS Text & Fonts

# CSS Text
CSS has a lot of properties for formatting text.

### Color
to Set the Text Color

```css
    h1{
        color: #000;
    }

```
### Background Color

to set background color of any element.
```css
h1{
    background-color: #afc;
}
```

### Text Alignment and Text Direction
Text Alignment
The text-align property is used to set the horizontal alignment of a text.

A text can be left or right aligned, centered, or justified.

```css
h1 {
  text-align: center;
}
```

### Text Direction & unicode-bidi
unicode-bidi roperties can be used to change the text direction of an element

### Vertical Alignment

vertical-align property sets the vertical alignment of an element.

## Text Decoration
Individual Text Decoration property

>text-decoration-line

>text-decoration-color

>text-decoration-style

>text-decoration-thickness

>text-decoration

```css
h1 {
  text-decoration-line: underline;
  text-decoration-thickness: auto;
}
```

Shorthand Property

```css
h1 {
  text-decoration: none;
}
```

### Text Transformation
property is used to specify uppercase and lowercase letters in a text.

```css
p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
```
### Text Spacing
text-indent
letter-spacing
line-height
word-spacing
white-space

```css
p {
  text-indent: 50px;
}
h1 {
  letter-spacing: 5px;
}
p.small {
  line-height: 0.8;
}
p.one {
  word-spacing: 10px;
}
p {
  white-space: nowrap;
}
```

### Text Shadow
property adds shadow to text.
In its simplest use, you only specify the horizontal shadow (2px) and the vertical shadow (2px):


```css
h1 {
  text-shadow: 2px 2px; /* also can add multiple values*/
    text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;

}
```

### CSS Fonts

font adds value to your text. It is also important to choose the correct color and text size for the font.
Font Selection is Important
Choosing right font has a huge impact.

### Generic Font Families
In CSS there are five generic font families:

#### Serif fonts:
have a small stroke at edges of each letter. They create a sense of formality and elegance.

#### Sans-serif:
fonts have clean lines (no small strokes attached). They create a modern and minimalistic look.

#### Monospace fonts:
all letters have the same fixed width. They create a mechanical look. 

#### Cursive fonts:
imitate human handwriting.

#### Fantasy fonts:
are decorative playful fonts.

All different font names belong to one of the generic font families. 

Difference Between Serif and Sans-serif Fonts

![FonT Selection](https://www.w3schools.com/css/serif.gif "Pic by w3school")


### CSS font-family Property

we use the font-family property to specify the font of a text.

```css
.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

```
## CSS Web Safe Fonts

Web safe fonts are fonts that are universally installed across all browsers and devices.

### Fallback Fonts
However, there are no 100% completely web safe fonts. There is always a chance that a font is not found or is not installed properly.

Therefore, it is very important to always use fallback fonts.

This means that you should add a list of similar "backup fonts" in the font-family property. If the first font does not work, the browser will try the next one, and the next one, and so on. Always end the list with a generic font family name.

```css
p {
font-family: Tahoma, Verdana, sans-serif;
}

```
Best Web Safe Fonts for HTML and CSS

few web safe fonts for HTML and CSS:

```css 
Arial (sans-serif)
Verdana (sans-serif)
Tahoma (sans-serif)
Trebuchet MS (sans-serif)
Times New Roman (serif)
Georgia (serif)
Garamond (serif)
Courier New (monospace)
Brush Script MT (cursive)
```

### CSS Font Fallbacks

Commonly Used Font Fallbacks
Below are some commonly used font fallbacks, organized by 5 generic font families:

```css
Serif
Sans-serif
Monospace
Cursive
Fantasy
```

### CSS Font Style

Font Style
font-style property is mostly used to specify italic text.

This property has three values:

normal - text is shown normally
italic - text is shown in italics
oblique - text is "leaning" (oblique is very similar to italic, but less supported)

```css
p.normal {
  font-style: normal;
}
```

### Font Weight
font-weight property specifies  weight of a font:
```css
p.normal {
  font-weight: normal;
}
```
### Font Variant
font-variant property specifies whether or not a text should be displayed in a small-caps font.
```css
p.normal {
  font-variant: normal;
}
```

### CSS Font Size
 font-size property sets the size of the text.

Being able to manage the text size is important in web design. However, we should not use font size adjustments to make paragraphs look like headings, or headings look like paragraphs.

Always use the proper HTML tags, like `<h1>` - `<h6>` for headings and `<p>` for para

### Absolute size:

Sets text to a specified size
Does not allow a user to change text size in all browsers.

Absolute size is useful when physical size of the output is known

### Relative size:

Sets the size relative to surrounding elements
Allows a user to change text size in browsers

Set Font Size With Pixels
Setting text size with pixels gives you full control over the text size:

```css
h1 {
  font-size: 40px;
}
```

Set Font Size With `Em`
To allow users to resize text , many developers use em instead of pixels.

`1em` is equal to the current font size. The default text size in browsers is 16px. So, the default size of 1em is 16px.

size can be calculated from pixels to em using this formula: pixels/16=em

```css
h1 {
  font-size: 2.5em; /* 40px/16=2.5em */
}

```

Use a Combination of Percent and Em
The solution that works in all browsers, is to set a default font-size in percent for `<body>` element:

```css
body {
  font-size: 100%;
}

h1 {
  font-size: 2.5em;
}

h2 {
  font-size: 1.875em;
}

p {
  font-size: 0.875em;
}
```

### Responsive Font Size
text size can be set with a vw unit, which means the "viewport width".

That way the text size will follow the size of the browser window:

```html
<h1 style="font-size:10vw">Hello World</h1>
```

### CSS Google Fonts

### Google Fonts
If you do not want to use any of the standard fonts in HTML, you can use Google Fonts.

Google Fonts are free to use, and have more than 1000 fonts to choose from.

How To Use Google Fonts
Just add a special style sheet link in the `<head>` section and then refer to the font in the CSS.

```html
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
}
</style>
</head>
```

### Use Multiple Google Fonts
To use multiple Google fonts, just separate the font names with a pipe character (|), like this:

```css
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">
<style>
h1.a {font-family: "Audiowide", sans-serif;}
h1.b {font-family: "Sofia", sans-serif;}
h1.c {font-family: "Trirong", serif;}
</style>
</head>
```

### Styling Google Fonts
Of course you can style Google Fonts as you like, with CSS!


### Enabling Font Effects
Google has also enabled different font effects that you can use.

First add effect=effectname to the Google API, then add a special class name to the element that is going to use the special effect. The class name always starts with font-effect- and ends with the effectname.

```html
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-fire">Sofia on Fire</h1>

</body>
```

CSS Great Font Pairings
