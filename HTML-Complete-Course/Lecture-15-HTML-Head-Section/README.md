### Head Element



`<head>` element is a container for metadata (data about data) and it is placed between the `<html>` tag and the `<body> `tag. it is a container for all of  these tags `<title>`, `<style>`, `<meta>`, `<link>`, `<script>`.. 

### What is Meta Data Data.
> HTML metadata is data about the HTML document

>Metadata define the document title, character set, styles, scripts, and other meta information.


HTML Favicon
How To Add a Favicon in HTML
A favicon is a small image displayed next to the page title in the browser tab.

You can use any image you like as your favicon. You can also create your own favicon on sites like https://www.favicon.cc.

Tip: A favicon is a small image, so it should be a simple image with high contrast.

A favicon image is displayed to the left of the page title in the browser tab, like this:

To add a favicon to your website, either save your favicon image to the root directory of your webserver, or create a folder in the root directory called images, and save your favicon image in this folder. A common name for a favicon image is "favicon.ico".

Next, add a <link> element to your "index.html" file, after the <title> element, like this:
Example
<!DOCTYPE html>
<html>
<head>
  <title>My Page Title</title>
  <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

Now, save the "index.html" file and reload it in your browser. Your browser tab should now display your favicon image to the left of the page title.


The HTML <title> Element
The <title> element defines the title of the document. The title must be text-only, and it is shown in the browser's title bar or in the page's tab.

The <title> element is required in HTML documents!

The content of a page title is very important for search engine optimization (SEO)! The page title is used by search engine algorithms to decide the order when listing pages in search results.

The <title> element:

defines a title in the browser toolbar
provides a title for the page when it is added to favorites
displays a title for the page in search engine-results
So, try to make the title as accurate and meaningful as possible!

A simple HTML document:
Example
<!DOCTYPE html>
<html>
<head>
  <title>A Meaningful Page Title</title>
</head>
<body>

The content of the document......

</body>
</html>


The HTML <style> Element
The <style> element is used to define style information for a single HTML page:

Example
<style>
  body {background-color: powderblue;}
  h1 {color: red;}
  p {color: blue;}
</style>

The HTML <link> Element
The <link> element defines the relationship between the current document and an external resource.

The <link> tag is most often used to link to external style sheets:

Example
<link rel="stylesheet" href="mystyle.css">

The HTML <meta> Element
The <meta> element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings.

The metadata will not be displayed on the page, but is used by browsers (how to display content or reload page), by search engines (keywords), and other web services.

Examples
Define the character set used:

<meta charset="UTF-8">
Define keywords for search engines:

<meta name="keywords" content="HTML, CSS, JavaScript">
Define a description of your web page:

<meta name="description" content="Free Web tutorials">
Define the author of a page:

<meta name="author" content="John Doe">
Refresh document every 30 seconds:

<meta http-equiv="refresh" content="30">
Setting the viewport to make your website look good on all devices:

<meta name="viewport" content="width=device-width, initial-scale=1.0">
Example of <meta> tags:

Example
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="John Doe">


Setting The Viewport
The viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.

You should include the following <meta> element in all your web pages:

<meta name="viewport" content="width=device-width, initial-scale=1.0">
This gives the browser instructions on how to control the page's dimensions and scaling.

The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

Here is an example of a web page without the viewport meta tag, and the same web page with the viewport meta tag:

Tip: If you are browsing this page with a phone or a tablet, you can click on the two links below to see the difference.

The HTML <script> Element
The <script> element is used to define client-side JavaScripts.

The following JavaScript writes "Hello JavaScript!" into an HTML element with id="demo":

Example
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
}
</script>

Tip: To learn all about JavaScript, visit our JavaScript Tutorial.

The HTML <base> Element
The <base> element specifies the base URL and/or target for all relative URLs in a page.

The <base> tag must have either an href or a target attribute present, or both.

There can only be one single <base> element in a document!

Example
Specify a default URL and a default target for all links on a page:

<head>
<base href="https://www.w3schools.com/" target="_blank">
</head>

<body>
<img src="images/stickman.gif" width="24" height="39" alt="Stickman">
<a href="tags/tag_base.asp">HTML base Tag</a>
</body>

Chapter Summary
The <head> element is a container for metadata (data about data)
The <head> element is placed between the <html> tag and the <body> tag
The <title> element is required and it defines the title of the document
The <style> element is used to define style information for a single document
The <link> tag is most often used to link to external style sheets
The <meta> element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings
The <script> element is used to define client-side JavaScripts
The <base> element specifies the base URL and/or target for all relative URLs in a page