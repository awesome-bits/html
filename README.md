# Metadata

Metadata contains information about the page. This includes information about styles, scripts and data to help software (search engines, browsers, etc.) use and render the page. Metadata for styles and scripts may be defined in the page or linked to another file that has the information.

## Head

The head element contains metadata about the page. This includes information about styles, scripts and data to help software (search engines, browsers, etc.) use and render the page. Metadata for styles and scripts may be defined in the page or linked to another file that has the information.

```html
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta charset="utf-8">
  <title>Page Title</title>
</head>
```

## Meta

The meta element contains metadata about the page. This includes information about styles, scripts and data to help software (search engines, browsers, etc.) use and render the page. Metadata for styles and scripts may be defined in the page or linked to another file that has the information.

```html
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
```

## Title

The title element defines the title of the page. This is the text that appears in the browser tab and is used by search engines to describe the page.

```html
<title>Page Title</title>
```

## Link

The link element defines a relationship between the page and another resource. This is commonly used to link to stylesheets and scripts.

```html
<link rel="stylesheet" href="style.css">
```

## Styles

Styles are used to define the look and feel of the page. This includes colors, fonts, spacing, etc. Styles can be defined in the page or linked to another file that has the information.

```html
<style>
  body {
    background-color: #fff;
    color: #000;
    font-family: sans-serif;
  }
</style>
```

## Scripts

Scripts are used to define the behavior of the page. This includes how the page responds to user interaction, how the page loads, etc. Scripts can be defined in the page or linked to another file that has the information.

```html
<script>
  console.log('Hello World!');
</script>

<script src="script.js"></script>
```

## Base

The base element defines the base URL for all relative URLs in the page. This is commonly used to define the base URL for all relative links and scripts.

```html
<head>
  <base href="https://example.com/">
</head>

<body>
  <a href="about">About</a>
  <script src="script.js"></script>
</body>
```