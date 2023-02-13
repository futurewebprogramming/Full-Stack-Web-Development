# Lecture -15

### Head Section of HTML Document.

### Head Element

`<head>` element is a container for metadata (information that describes the content of a web page) that is not displayed directly on the page.  `<head>` element should appear at the beginning of every HTML document, immediately after the `<html>` tag.

Here is an example of the `<head>` element in an HTML document:

```html
<html>
  <head>
    <title>Example Page</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="styles.css">
      <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
  </head>
  <body>
    <!-- The main content of the page goes here -->
  </body>
</html>
```
#### `<head>` element 
`<head>` element  can contain the following elements:

#### `<title>` element: 
specifies the title of the document, which is displayed in the browser's title bar or tab.
#### `<meta>` Element: 
provides metadata about the document, such as a description of the content, keywords for search engines, character encoding, and viewport settings.
#### `<link>`: 
specifies relationships between the document and external resources, such as favicon, stylesheets and scripts.
### HTML Favicon

favicon is a small, iconic image that represents a website or a web page. In HTML, a favicon is typically added to a web page by including a `<link>` element within the `<head>` section of the document.  `<link> `element specifies the location of the favicon file and the relationship between the document and the favicon.
```html
<html>
  <head>
    <title>Example Page</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="styles.css">
    <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
  </head>
  <body>
    <!-- The main content of the page goes here -->
  </body>
</html>
```

### `<link>` for Fav Icon Attributes
#### rel attribute
 is set to "shortcut icon" to indicate the relationship between the document and the favicon. 
#### type attribute
specifies the file type of the favicon, which is "image/x-icon" for ICO files. 
#### href attribute 
specifies the location of the favicon file.

>we can use any image you like as your favicon. You can also create your own favicon on sites like https://www.favicon.cc.


```html

<meta charset="UTF-8">
Define the character set used:

>"UTF-8" character set is a type of character encoding 
that represents the text on a web page 
using a standardized set of characters.
 UTF-8 stands for "Unicode Transformation Format 8-bit"
and is a widely-used character encoding 
that supports a large number of characters
from many different languages and scripts.

By specifying the character set as UTF-8 in the meta element, 
the web page is telling the browser to 
expect text encoded in UTF-8 and to render
it accordingly. This helps ensure that the
text is displayed correctly, 
regardless of the language or script used.

<meta name="keywords" content="HTML, CSS, JavaScript">
Define keywords for search engines:

<meta name="description" content="Free Web tutorials">
Define a description of your web page:

<meta name="author" content="John Doe">
Define the author of a page:

<meta http-equiv="refresh" content="30">
Refresh document every 30 seconds:

<meta name="viewport" content="width=device-width, initial-scale=1.0">
Setting the viewport to make your website look good on all devices:
```
Eample:
```html
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="John Doe">
```

### Setting The Viewport
viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
This gives the browser instructions on how to control the page's dimensions and scaling.

#### width=device-width 
>part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

#### initial-scale=1.0 
>part sets the initial zoom level when the page is first loaded by the browser.


### HTML `<script>` Element
`<script>` element is used to define client-side JavaScripts.

```html
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
}
</script>
```
