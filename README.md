# Multimedia Elements

HTML supports a number of multimedia elements. 

## Image

The HTML `<img>` element is used to embed an image in a web page. Images are not technically inserted into a web page; images are linked to web pages. The `<img>` element creates a holding space for the referenced image.

The `<img>` tag has two common attributes:

- src - Specifies the path to the image
- alt - Specifies an alternate text for the image

The `src` attribute is required, and contains the path to the image you want to embed. The `alt` attribute is optional, but recommended, and provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the `src` attribute, or if the user uses a screen reader).

```html
<img src="logo.png" alt="Logo">
```

## Audio

The HTML `<audio>` element is used to embed sound content in a document, such as music or other audio streams.

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
```

## Video

The HTML `<video>` element is used to show a video on a web page.

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

## Figure

The HTML `<figure>` element represents self-contained content, frequently with a caption (`<figcaption>`), and is typically referenced as a single unit. While it is related to the main flow, its position is independent of the main flow. Usually this is an image, an illustration, a diagram, a code snippet, or a schema that is referenced in the main text, but that can be moved to another page or to an appendix without affecting the main flow.

```html
<figure>
  <img src="https://www.w3schools.com/html/pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>
```

## Map

The HTML `<map>` element is used with `<area>` elements to define an image map (a clickable link area).

```html
<map>
  <area shape="rect" coords="0,0,82,126" href="sun.htm" alt="Sun">
  <area shape="circle" coords="90,58,3" href="mercur.htm" alt="Mercury">
  <area shape="circle" coords="124,58,8" href="venus.htm" alt="Venus">
</map>
```
