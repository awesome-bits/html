# Inline Text Elements

Use the HTML inline text semantic to define the meaning, structure, or style of a word, line, or any arbitrary piece of text.

## Anchor

The anchor element creates a hyperlink to other web pages, files, locations within the same page, email addresses, or any other URL.

```html
<a href="https://www.google.com">Google</a>
```

## Abbreviation

The abbreviation element represents an abbreviation or acronym; the optional title attribute can provide an expansion or description for the abbreviation.

```html
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```

## Bold

The bold element represents a span of text stylistically different from normal text, without conveying any special importance or relevance.

```html
<p><b>bold text</b></p>
```

## Bidirectional Isolation

The bidirectional isolation element represents a span of text that is isolated from its surroundings for the purposes of bidirectional text formatting.

```html
<p>Here is some <bdi>RTL text</bdi> embedded in LTR text.</p>
```

## Override Bidirectional Algorithm

The override bidirectional algorithm element overrides the current directionality of text, so that the text within is rendered in a different direction.

```html
<p>Here is some <bdo dir="rtl">RTL text</bdo> embedded in LTR text.</p>
```

## Cite

The cite element represents the title of a work (e.g. a book, a paper, an essay, a poem, a score, a song, a script, a film, a TV show, a game, a sculpture, a painting, a theatre production, a play, an opera, a musical, an exhibition, a legal case report, etc). This can be a work that is being quoted or referenced in detail (i.e. a citation), or it can just be a work that is mentioned in passing.

```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```

## Code

The code element represents a fragment of computer code. By default, it is displayed in the browser's default monospace font.

```html
<p>Use the <code>git clone</code> command.</p>
```

## Data

The data element represents its contents, along with a machine-readable form of those contents in the value attribute.

```html
<p>My name is <data value="John Doe">JD</data>.</p>
```

## Definition

Definition element represents the defining instance of a term.

```html
<p><dfn>HTML</dfn> is the standard markup language for creating web pages.</p>
```

## Deleted Text

The deleted text element represents a range of text that has been deleted from a document.

```html
<p><del>deleted text</del></p>
```

## Emphasis

The emphasis element represents a span of text with emphatic stress. By default, this is text that is displayed in italic.

```html
<p><em>emphasized text</em></p>
```

## Italic

The italic element represents a span of text that is set off from the normal text for some reason. By default, this is text that is displayed in italic.

```html
<p><i>italic text</i></p>
```

## Keyboard

The keyboard element represents user input (typically keyboard input, although it may also be used to represent other input, such as voice commands).

```html
<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text.</p>
```

## Mark

The mark element represents text which is marked or highlighted for reference or notation purposes, due to the marked passage's relevance or importance in the enclosing context.

```html
<p>Use the <mark>mark</mark> element to <mark>highlight</mark> text.</p>
```

## Quote

The quote element represents some phrasing content quoted from another source.

```html
<p>Use the <q>quote</q> element to <q>quote</q> text.</p>
```

## Ruby

The ruby element represents a ruby annotation. Ruby annotations are for showing pronunciation of East Asian characters.

```html
<p>漢字 <ruby>漢 <rp>(</rp><rt>かん</rt><rp>)</rp></ruby> 字 <ruby>字 <rp>(</rp><rt>じ</rt><rp>)</rp></ruby></p>
```

## Strikethrough

The strikethrough element represents a range of text that has been deleted from a document.

```html
<p><s>strikethrough text</s></p>
```

## Sample

The sample element represents sample or quoted output from another program or computing system.

```html
<p>Use the <samp>git clone</samp> command.</p>
```

## Small

The small element represents side comments such as small print.

```html
<p><small>small text</small></p>
```

## Strong

The strong element represents strong importance, seriousness, or urgency for its contents.

```html
<p><strong>strong text</strong></p>
```

## Subscript

The subscript element represents a subscript.

```html
<p>Water is composed of two elements, hydrogen (<sub>H</sub>) and oxygen (<sub>O</sub>).</p>
```

## Superscript

The superscript element represents a superscript.

```html
<p>E=mc<sup>2</sup></p>
```

## Time

The time element represents either a time on a 24-hour clock or a precise date in the Gregorian calendar (with optional time and timezone information).

```html
<p>My birthday is <time datetime="2000-01-01">January 1st 2000</time>.</p>
```

## Underline

The underline element represents a span of text stylistically different from normal text, without conveying any special importance or relevance.

```html
<p><u>underlined text</u></p>
```

## Variable

The variable element represents the name of a variable in a mathematical expression or a programming context.

```html
<p><var>w</var> × <var>h</var></p>
```

## Word Break Opportunity

The word break opportunity element represents a position within text where the browser may optionally break a line, though its line-breaking rules would not otherwise create a break at that location.

```html
<p>Here is some text that might <wbr>wrap.</p>
```