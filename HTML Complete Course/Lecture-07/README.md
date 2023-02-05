# Lecture -07

## HTML Links Explained

### What are links  ?

We already have discussed links in our previous lecture, but in this lecture we will study in detail about links.

HTML links allow you to connect your web pages together, and to other web pages on the internet. Here's how you can create links in HTML:

Also let me again expalain about
`Absolute URLs vs. Relative URLs` with Example.

>Absolute URLs are External Links of Any Website 

```html
<h3>Absolute URLs</h3>
<p><a href="https://google.com/">Google</a></p>
<p><a href="https://developer.mozilla.org/">MDN</a></p>
```

>Relative URLs are Internal Links within your Website.

```html
<h3>Relative URLs</h3>
<p><a href="about.html">About US</a></p>
<p><a href="../services.html/">Services</a></p>
```

#### Linking to other pages

You can link to other pages on your website by using relative paths. For example, if you have a file named "`about.html`" in the same directory as the current page, you can link to it using the following code:

```html
<a href="about.html">About</a>
```

#### Linking to specific parts of a page

You can link to specific parts of a page by using the `id` attribute. For example, you can create a named anchor on a page like this:

```html
<a id="top">Top of the Page</a>
```

And then link to it from another page or from another part of the same page like this:

```html
<a href="#top">Go to Top</a>
```

#### Linking to email addresses

 You can create a link that will open the user's email client and pre-populate the "To" field with an email address. Use the following syntax:

```html
<a href="mailto:example@example.com">Send Email</a>
```

#### Opening links in a new tab

 You can specify that a link should open in a new tab by using the target attribute and setting it to "`_blank`".

#### Use an Image as a Link

```html
<a href="https://google.com">
<img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="Google" style="width:42px;height:42px;">
</a>
```

Button as a Link

```js
<button onclick="document.location='/practice.html'">Do Practice</button>

```
