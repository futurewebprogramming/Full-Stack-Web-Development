# Lecture -05

## HTML Styles  Text formating

> HTML style attribute is used to add styles to an element, such as color, font, size, and more.

```html
<tagname style="property:value;"></tagname>
```

> The property is a CSS property. The value is a CSS value.

### Background Color

<p
style="background-color:blue;
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

### HTML Formatting Elements

> Formatting elements were designed to display special types of text

```html
<b>
  - Bold text
  <strong>
    - Important text
    <i>
      - Italic text
      <em>
        - Emphasized text
        <mark>
          - Marked text
          <small>
            - Smaller text
            <del>
              - Deleted text
              <ins>
                - Inserted text
                <sub> - Subscript text <sup> - Superscript text</sup></sub></ins
              ></del
            ></small
          ></mark
        ></em
      ></i
    ></strong
  ></b
>
```

<b> - Bold text </b>

> <b> element defines bold text, without any extra importance.

<strong> - Important text </strong>

> HTML <strong> element defines text with strong importance.

<i> - Italic text</i>

> <i> Italsize text in italic without emphasis

<em> emphasized Text </em>

> `<em>` element defines emphasized text

> A screen reader will pronounce the words `<em>` with emphasis, using verbal stress.

<mark> - Marked text </mark>

> `<mark>`element defines text that should be marked or highlighted

<small> - Smaller text </small>

> `<small>` element defines smaller text

<del> - Deleted text </del>

> `<del>` Browsers Showes strike a line through deleted text

<ins> - Inserted text </ins>

> HTML`<ins>` element defines a text that has been inserted into a document like Mango Price is <del>100$</del> <ins>80$</ins>.</p>

<sub> - Subscript text </sub>

> Subscript text appears half a character below the normal line like
> H<sub> 2 </sub>O

<sup> - Superscript text </sup>

> Superscript text appears half a character above the normal line like H<sup> 2 </sup>O

> `<blockquote>` element defines a section that is quoted from another source and Browsers usually indent `<blockquote> elements` like down below

<blockquote> Patience is a key element of success. </blockquote>

### `<q>` Tag

> `<q>` tag defines a short quotation

<q>Patience is a key element of success.</q>

### `<abbr>` for Abbreviations

> we use `<abbr>` with _**title**_ attibute for Abbreviations like "HTML", "CSS", "JS",, etc.

<abbr
title="Hyper Text Markup Language">HTML</abbr>

<abbr
title="Cascading Style Sheet">CSS
</abbr>

<abbr
title="Javascript">Js
</abbr>

### `<address>` for Contact Information

> we use for contact information and contact can be an email address, URL, physical address, phone number, social media handle, etc.

> for example:

<address>
Written by Jhon Doe.<br>
Visit us at: <br> 
Future Programming youtube.com<br>
Box 564, Disneyland<br>
USA
</address>

### `<cite>` Tag

>`<cite>` tag defines the title of a creative work (e.g a book, a poem, a song, a movie, a painting, a sculpture, etc.).

for example:

<img src="https://th.bing.com/th/id/OIP.yCEFQDme4_a34fhpUDnJjwHaKd?pid=ImgDet&rs=1" width=400px height=300px>

<cite>The Rail</cite> 
Oil Painting by Jhon Doe

#### `<bdo>` for Bi-Directional Override
>to change/override current text direction

<bdo dir="rtl">This line will be written from right to left</bdo>

