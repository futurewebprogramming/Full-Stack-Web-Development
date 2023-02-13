## Lecture 14.

#### Sementic Element VS Non Sementic Elements

[![Source DEV.to](https://res.cloudinary.com/practicaldev/image/fetch/s--7rtr6qdB--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/n8f7yj3bjy7rcu03hfsa.png "Non Sementic HTML vs Sementic HTML pic by Dev.to himanshu gupta")](https://dev.to/himanshudevgupta/html-semantic-tag-vs-non-semantic-2fj3#:~:text=Non-semantic%20HTML%20refers%20to%20the%20use%20of%20HTML,about%20the%20meaning%20or%20purpose%20of%20that%20content.)


Semantic elements and non-semantic elements are terms used to describe different types of HTML elements in a web page.


Semantic elements
>elements with a meaning.

Semantic elements are HTML elements that have a `specific meaning` and purpose. They describe the content they contain, making it `easier` for `browsers`, `search engines`, and assistive technologies to _**understand the structure and purpose**_ of a web page. Examples of semantic elements include:

```html
<header> - defines the header of a document or section (element represents a container for introductory content or a set of navigational links)
<nav> - defines a section for navigation links
<main> - defines the main content of a document
<article> - defines a self-contained article
<section> - defines a standalone section of a document
<aside> - defines content aside from the main content
<footer> - defines the footer of a document or section

```

### Non Sementic Elements
>Tells nothing about its content.

Non-semantic elements, on the other hand, do not have a specific meaning or purpose. They are used for styling and layout purposes only and do not convey any information about the content they contain. Examples of non-semantic elements include:
```html
<div> - a generic container for flow content
<span> - a generic inline container for flow content
<hr> - defines a horizontal rule for visual separation of content
```
### Why Semantic Elements?

In general, it is `recommended` to `use semantic elements` _**whenever possible**_ to provide meaningful information about the content and structure of a web page. Non-semantic elements should be used only when there is no semantic element that fits the purpose.


### HTML Section Element
`<section>` element defines a section in a document page.

>Examples of where a `<section>` element can be used:

```html
Chapters,
Introduction,
News items,
Contact information
```

>A web page could normally be split into sections for introduction, content, and contact information.


### `<article>` Element

`<article>` element specifies independent, self-contained content.

>An article should make sense on its own, and it should be possible to distribute it independently from the rest of the web site.

Examples of where the `<article>` element can be used:

```html
Forum posts
Blog posts
User comments
Product cards
Newspaper articles
```

```html
<article class="all-browsers">
  <h1>Most Popular Browsers</h1>
  <article class="browser">
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
  </article>
  <article class="browser">
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
  </article>
  <article class="browser">
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
  </article>
</article>
```

### `<header>` Element
`<header>` element represents a container for introductory content or a set of navigational links.

```html
<article>
  <header>
    <h1>What Does WWF Do?</h1>
    <p>WWF's mission:</p>
  </header>
  <p>WWF's mission is to stop the degradation of our planet's natural environment,
  and build a future in which humans live in harmony with nature.</p>
</article>
HTML <footer> Element
The <footer> element defines a footer for a document or section.
```
### `<footer>` element 
```html
authorship information
copyright information
contact information
sitemap
back to top links
related documents
```
```html
<footer>
  <p>Author: Hege Refsnes</p>
  <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer>
```
### HTML `<nav>` Element
`<nav>` element defines a set of navigation links.

```html
<nav>
  <a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav>
```
### `<aside>` Element
`<aside>` element defines some content aside from the content it is placed in (like a sidebar).

```html
<html>
<head>
<style>
aside {
  width: 30%;
  padding-left: 15px;
  margin-left: 15px;
  float: right;
  font-style: italic;
  background-color: lightgray;
}
</style>
</head>
<body>

<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
<p>The Epcot center is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>

<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

</body>
</html>
```
### `<figure>` and `<figcaption>` Elements

`<figure>` tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

`<figcaption>` tag defines a caption for a `<figure>` element. 

`<img>` element defines the actual image/illustration. 

```html
<figure>
  <img src="pic_trulli.jpg" alt="Trulli">
  <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure>
```
