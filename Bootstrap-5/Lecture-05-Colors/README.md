# Lecture -05  Colors and Background Colors

## Text Colors
Bootstrap 5 has some contextual classes that can be used to provide "meaning through colors".

The classes for text colors are: 

```css 
.text-muted, .text-primary, .text-success, .text-info, .text-warning, .text-danger, .text-secondary, .text-white, .text-dark, .text-body (default body color/often black) and .text-light:

```
Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Contextual Colors</h2>
  <p>Use the contextual classes to provide "meaning through colors":</p>
  <p class="text-muted">This text is muted.</p>
  <p class="text-primary">This text is important.</p>
  <p class="text-success">This text indicates success.</p>
  <p class="text-info">This text represents some information.</p>
  <p class="text-warning">This text represents a warning.</p>
  <p class="text-danger">This text represents danger.</p>
  <p class="text-secondary">Secondary text.</p>
  <p class="text-dark">This text is dark grey.</p>
  <p class="text-body">Default body color (often black).</p>
  <p class="text-light">This text is light grey (on white background).</p>
  <p class="text-white">This text is white (on white background).</p>
</div>

</body>
</html>

```

You can also add 50% opacity for black or white text with the .text-black-50 or .text-white-50 classes:

Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Opacity Text Colors</h2>
  <p>Add 50% opacity for black or white text with the .text-black-50 or .text-white-50 classes:</p>
  <p class="text-black-50">Black text with 50% opacity on white background</p>
  <p class="text-white-50 bg-dark">White text with 50% opacity on black background</p>
</div>

</body>
</html>

```
## Background Colors


The classes for background colors are: 


```css
.bg-primary, .bg-success, .bg-info, .bg-warning, .bg-danger, .bg-secondary, .bg-dark and .bg-light.
```
Example
The .bg-color classes above does not work well with text, or atleast then you have to specify a proper .text-color class to get the right text color for each background.

However, you can use the .text-bg-color classes and Bootstrap will automatically handle the appropriate text color for each background color:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Contextual Backgrounds</h2>
  <p>Use the contextual background classes to provide "meaning through colors".</p>
  <div class="bg-primary p-3"></div>
  <div class="bg-success p-3"></div>
  <div class="bg-info p-3"></div>
  <div class="bg-warning p-3"></div>
  <div class="bg-danger p-3"></div>
  <div class="bg-secondary p-3"></div>
  <div class="bg-dark p-3"></div>
  <div class="bg-light p-3"></div>
</div>

</body>
</html>


```