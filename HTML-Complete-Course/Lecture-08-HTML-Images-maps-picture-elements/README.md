# Lecture -08

## HTML images, Image Map , Picture Element

HTML images are used to display images on a web page. Here's how you can add images in HTML:

### Image tag `<img>`

 The image tag is used to embed images in a web page. You can specify the source of the image using the src attribute and the alternate text for the image using the alt attribute.

```html
<img src="image.jpg" alt="Description of the image">
```

### Image size

You can specify the size of an image using the width and height attributes. These attributes can be set in pixels or as a percentage of the available space.

```html
<img src="image.jpg" alt="Description of the image" width="100" height="100">
```

#### Image alignment

You can align an image to the left, right, or center of the web page using CSS.

```html
 <img src="image.jpg" alt="Description of the image" style="float:right;">

```

#### Image as a link

You can make an image a clickable link by wrapping the image tag inside an anchor tag.

```html
<a href="http://www.example.com">
  <img src="image.jpg" alt="Description of the image">
</a>
```

### Image as a BackGround

>A background image can be specified for almost any HTML element.

```html
<p style="background-image: url('img_girl.jpg');">
```

#### Image formats

The most common image formats for web use are `JPEG, PNG, and GIF and WebP`. Choose the format that is best for your needs based on the type of image and the desired quality and file size


### HTML Maps

HTML image maps allow you to associate multiple hyperlinks with different parts of a single image. Here's how you can create image maps in HTML:

### Map tag `<map>`

The map tag is used to `define` the `image map`. You can give the map a unique name using the `name attribute`, and then associate the map with an image using the `usemap` attribute.

```html
<img src="image.jpg" alt="Description of the image" usemap="#mapname">
```

```html
<map name="mapname">
<area shape="rect" coords="10,10,50,50" href="http://www.example.com">
</map>
```

### Area tag `<area>`

The area tag is used to define clickable regions within the image map. You can specify the `shape` and size of the region using the shape and `coords` attributes, and the destination of the link using the `href` attribute.

```html
<area shape="rect" coords="10,10,50,50" href="http://www.example.com">
```

### Shapes

The available shapes for image maps are `rectangle`, `circle`, and `polygon`. You can specify the shape using the `shape` attribute, and the coordinates of the shape using the coords attribute.

`Rectangle Region`: shape="rect" coords="x1,y1,x2,y2"

`Circle`: shape="circle" coords="x,y,r"

`Polygon Region`: shape="poly" coords="x1,y1,x2,y2,x3,y3,..."

### Pituce Element

The HTML `<picture>` element is used to provide _**multiple sources**_ for an image to adapt to _**different devices**_ and display conditions. The `< picture>` element enables you to define multiple sources for an image, and the browser will choose the best source to display based on the media attribute of each `< source>` element.

Here's an example of how to use the

### Picture> element

```html
<picture>
  <source srcset="image-small.jpg" media="(max-width: 767px)">
  <source srcset="image-large.jpg" media="(min-width: 768px)">
  <img src="image-default.jpg" alt="Description of the image">
</picture>
```

In this example, the `< picture>` element contains two `< source>` elements and an `< img>` element.

The _**srcset attribute**_ of each `< source>` element specifies the source of the image, and the _**media attribute**_ specifies the conditions under which that image should be used.
