# Lecture 13

## HTML Multimedia

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

Web pages often contain multimedia elements of different types and formats.

Multimedia Formats

Multimedia files have formats and different extensions like: .wav, .mp3, .mp4, .mpg, .wmv, and .avi.

HTML <video> Element
>show a video in HTML, use the <video> element:

HTML <video> element is used to show a video on a web page.

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>    
```

controls attribute adds video controls, like play, pause, and volume

It is a good idea to always include width and height attributes. 
If height and width are not set, the page might flicker while the video loads.

The <source> element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.

The text between the <video> and </video> tags will only be displayed in browsers that do not support the <video> element.

HTML <video> Autoplay
To start a video automatically, use the autoplay attribute:

<video width="320" height="240" autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>

Add muted after autoplay to let your video start playing automatically (but muted):

<video width="320" height="240" autoplay muted>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>


HTML Video - Methods, Properties, and Events

The HTML DOM defines methods, properties, and events for the <video> element.

This allows you to load, play, and pause videos, as well as setting duration and volume.

There are also DOM events that can notify you when a video begins to play, is paused, etc.


### HTML Audio

The HTML <audio> element is used to play an audio file on a web page.

### HTML <audio> Element

<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

HTML Audio - How It Works
The controls attribute adds audio controls, like play, pause, and volume.

The <source> element allows you to specify alternative audio files which the browser may choose from. The browser will use the first recognized format.

The text between the <audio> and </audio> tags will only be displayed in browsers that do not support the <audio> element.

HTML <audio> Autoplay
To start an audio file automatically, use the autoplay attribute:

Add muted after autoplay to let your audio file start playing automatically (but muted):

<audio controls autoplay muted>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

HTML Audio - Methods, Properties, and Events

he HTML DOM defines methods, properties, and events for the <audio> element.

This allows you to load, play, and pause audios, as well as set duration and volume.

There are also DOM events that can notify you when an audio begins to play, is paused, etc.

```html
<div style="text-align:center"> 
  <button onclick="playPause()">Play/Pause</button> 
  <button onclick="makeBig()">Big</button>
  <button onclick="makeSmall()">Small</button>
  <button onclick="makeNormal()">Normal</button>
  <br><br>
  <video id="video1" width="420">
    <source src="mov_bbb.mp4" type="video/mp4">
    <source src="mov_bbb.ogg" type="video/ogg">
    Your browser does not support HTML video.
  </video>
</div> 

<script> 
var myVideo = document.getElementById("video1"); 

function playPause() { 
  if (myVideo.paused) 
    myVideo.play(); 
  else 
    myVideo.pause(); 
} 

function makeBig() { 
    myVideo.width = 560; 
} 

function makeSmall() { 
    myVideo.width = 320; 
} 

function makeNormal() { 
    myVideo.width = 420; 
} 
</script> 

<p>Video courtesy of <a href="https://www.bigbuckbunny.org/" target="_blank">Big Buck Bunny</a>.</p>
```

HTML YouTube Videos
The easiest way to play videos in HTML, is to use YouTube.

Struggling with Video Formats?
Converting videos to different formats can be difficult and time-consuming.

An easier solution is to let YouTube play the videos in your web page.YouTube Video Id
YouTube will display an id (like tgbNymZ7vqY), when you save (or play) a video.

You can use this id, and refer to your video in the HTML code.

Playing a YouTube Video in HTML
To play your video on a web page, do the following:

Upload the video to YouTube
Take a note of the video id
Define an <iframe> element in your web page
Let the src attribute point to the video URL
Use the width and height attributes to specify the dimension of the player
Add any other parameters to the URL (see below)

<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>

YouTube Autoplay + Mute
You can let your video start playing automatically when a user visits the page, by adding autoplay=1 to the YouTube URL. However, automatically starting a video is annoying for your visitors!

Add mute=1 after autoplay=1 to let your video start playing automatically (but muted).

<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>

YouTube Playlist
A comma separated list of videos to play (in addition to the original URL).

YouTube Loop
Add loop=1 to let your video loop forever.

Value 0 (default): The video will play only once.

Value 1: The video will loop (forever).

YouTube - Loop

<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>

YouTube Controls
Add controls=0 to not display controls in the video player.

Value 0: Player controls does not display.

Value 1 (default): Player controls display.

<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?controls=0">
</iframe>