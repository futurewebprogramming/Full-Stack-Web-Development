# Lecture 13

## HTML Multimedia & I frames

# HTML Iframes

An HTML iframe is used to display a web page within a web page.


`<iframe> `tag specifies an inline frame.

```html
<iframe src="https://bing.com/" title="bing.com"></iframe>
```

We can Add iframe via Absoulte Path or Relative Path.

```html
<iframe src="practice.html" name=" practice"title="bing.com"></iframe>
<p><a href="practice.html" target="practice">Do Practice</a></p>
```

### Iframe Attribute: 

Height and Width on the iframe HTML Element or we add by style Attribute.

> Use height and width attributes to specify the size of the iframe.

```html
<iframe src="https://bing.com/" title="bing.com" width="100%" height="100%"></iframe>
```

### Remove the Border

By default, an iframe has a border around it. to remove border, add `border: none` css property


```html
<iframe src="https://bing.com/" title="bing.com" width="100%" height="100%" style="border:none"></iframe>
```

## Multimedia

Multimedia comes in many different formats. It can be almost anything you can hear or see, like images, music, sound, videos, records, films, animations, and more.

### Multimedia Formats:

Multimedia files have formats and different extensions like: .wav, .mp3, .mp4, .mpg, .wmv, and .avi.

HTML `<video>` Element
>show a video in HTML, use the `<video>` element:

HTML `<video>` element is used to show a video on a web page.

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
</video>    
```

### `<source>` element 
allows you to specify alternative video files which the browser may choose from.


###  Autoplay
To start a video automatically, use the autoplay attribute:

```html
<video width="320" height="240" autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
</video>
```
### Muted 
after autoplay to let your video start playing automatically

```html
<video width="320" height="240" autoplay muted>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
</video>
```
### HTML Audio

HTML `<audio>` element is used to play an audio file on a web page.

### HTML `<audio>` Element

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
</audio>
```


### HTML YouTube Videos

An easier solution is to let YouTube play the videos in your web page.YouTube Video Id
YouTube will display an id (like tgbNymZ7vqY), when you save (or play) a video.

You can use this id, and refer to your video in the HTML code.

```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```
### YouTube Autoplay + Mute
we can add it at the end of video url with `?` mark

`autoplay=1`
`mute=1 `

```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>
```
### YouTube Playlist

we will add like we add single video difference is we have to add  `loop` with `1` 0r `0` with & Symbol at the end of video url. 

#### YouTube Loop
##### loop=1 
to let your video loop forever.  

##### Value=0
 video will play only once.


```html
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```