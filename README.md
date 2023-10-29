# Embedded Content in HTML

In addition to regular multimedia content, you can embed content with other tags.

## Embed

Embeds external content at the specified point in the document. This content is provided by an external application or other source of interactive content such as a browser plug-in.

```html
<embed type="video/webm" src="/media/cc0-videos/flower.mp4" width="250" height="200" />
```

## Iframe

Represents a nested browsing context, effectively embedding another HTML page into the current page.

```html
<iframe src="https://example.org" width="560" height="315" frameborder="0" allowfullscreen></iframe>
```

## Object

Represents an external resource, which can be treated as an image, a nested browsing context, or a resource to be handled by a plugin.

```html
<object data="helloworld.swf" type="application/x-shockwave-flash">
  <param name="movie" value="helloworld.swf" />
  <param name="quality" value="high" />
</object>

<object data="helloworld.swf" type="application/x-shockwave-flash">
  <param name="movie" value="helloworld.swf" />
  <param name="quality" value="high" />
  <p>
    Alternative content
  </p>
</object>
```

## Picture

Represents a container for multiple image sources.

```html
<picture>
  <source srcset="/media/cc0-images/surfer-240-200.jpg" media="(orientation: portrait)" />
  <img src="/media/cc0-images/painted-hand-298-332.jpg" alt="" />
</picture>
```

## Portal

Represents a portal, an HTML element whose contents are embedded in a different document.

```html
<portal src="https://example.com/">
  <p>Portal content</p>
</portal>
```
