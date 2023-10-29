# Text Layout

## Headings h1 to h6

Headings in html are defined by the `<h1>` to `<h6>` tags. 

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
```

hgroup is used to group headings together.

```html
<hgroup>
  <h1>Heading 1</h1>
  <h2>Heading 2</h2>
</hgroup>

## Paragraphs

Paragraphs are defined by the `<p>` tag.

```html
<p>Paragraph 1</p>
<p>
  lorem ipsum dolor sit amet, consectetur adipiscing elit.
</p>
```

## Blockquotes

Blockquotes are defined by the `<blockquote>` tag. It is used to quote text from another source.

```html
<blockquote cite="https://datatracker.ietf.org/doc/html/rfc1149">
  <p>
    Avian carriers can provide high delay, low throughput, and low altitude
    service. The connection topology is limited to a single point-to-point path
    for each carrier, used with standard carriers, but many carriers can be used
    without significant interference with each other, outside early spring. This
    is because of the 3D ether space available to the carriers, in contrast to
    the 1D ether used by IEEE802.3. The carriers have an intrinsic collision
    avoidance system, which increases availability.
  </p>
</blockquote>
```

## Lists

Lists are defined by the `<ul>` and `<ol>` tags. `<ul>` is used for unordered lists and `<ol>` is used for ordered lists. `<li>` is used to define each list item.

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

## Description Lists

Description lists are defined by the `<dl>` tag. `<dt>` is used to define the term and `<dd>` is used to define the description.

```html
<dl>
  <dt>Term 1</dt>
  <dd>Description 1</dd>
  <dt>Term 2</dt>
  <dd>Description 2</dd>
</dl>
```

## Menu

Menu is defined by the `<menu>` tag. It is used to define a list of commands. The difference between `<menu>` and `<ul>` is that `<menu>` is used to define a list of commands while `<ul>` is used to define a list of items.

```html
<menu>
  <li>Item 1</li>
  <li>Item 2</li>
</menu>
```

## Address

Address is defined by the `<address>` tag. It is used to define the contact information of the author of the document.

```html
<address>
  <p>John Doe</p>
  <p>
    1234 Main St<br />
    Anytown, CA 12345<br />
    USA
  </p>
</address>
```

## Preformatted Text

Preformatted text is defined by the `<pre>` tag. It is used to define text that is already formatted. The text inside the `<pre>` tag is displayed in a fixed-width font and the text preserves both spaces and line breaks.

```html
<pre>
  function helloWorld() {
    console.log("Hello World!");
  }

  helloWorld();
</pre>
```

[Back](../../tree/main)