# Vector Graphics

## SVG
The svg element is a container that defines a new coordinate system and viewport.

```html
<svg width="100" height="100">
</svg>
```

## Circle

```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

## Rectangle

```html
<svg width="100" height="100">
  <rect x="10" y="10" width="80" height="80" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

## Line

```html
<svg width="100" height="100">
  <line x1="10" y1="10" x2="90" y2="90" stroke="green" stroke-width="4" />
</svg>
```

## Polyline

```html
<svg width="100" height="100">
  <polyline points="10,10 90,10 90,90" stroke="green" stroke-width="4" fill="none" />
</svg>
```

## Polygon

```html
<svg width="100" height="100">
  <polygon points="10,10 90,10 90,90" stroke="green" stroke-width="4" fill="none" />
</svg>
```

## Path

```html
<svg width="100" height="100">
  <path d="M10,10 L90,10 L90,90" stroke="green" stroke-width="4" fill="none" />
</svg>

<svg width="100" height="100">
  <path d="M10,10 L90,10 L90,90 Z" stroke="green" stroke-width="4" fill="none" />
</svg>

<svg width="100" height="100">
  <path d="M10,10 L90,10 L90,90 Z M50,50 L90,50 L90,90" stroke="green" stroke-width="4" fill="none" />
</svg>

<svg width="100" height="100">
  <path d="M10,10 L90,10 L90,90 Z M50,50 L90,50 L90,90" stroke="green" stroke-width="4" fill="none" />
</svg>
```

## Text

```html
<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="rotate(30, 20, 40)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="translate(20, 40)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="scale(2, 1)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="skewX(30)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="skewY(30)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="matrix(1, 0.5, 0, 1, 0, 0)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="rotate(30, 20, 40) translate(20, 40) scale(2, 1) skewX(30) skewY(30) matrix(1, 0.5, 0, 1, 0, 0)">Hello</text>
</svg>

<svg width="100" height="100">
  <text x="10" y="50" font-family="Verdana" font-size="35" fill="blue" transform="rotate(30, 20, 40) translate(20, 40) scale(2, 1) skewX(30) skewY(30) matrix(1, 0.5, 0, 1, 0, 0)">Hello</text>
</svg>
```

## Image

```html
<svg width="100" height="100">
  <image xlink:href="https://www.w3.org/TR/SVG/images/painting/fill01.svg" x="0" y="0" width="100" height="100" />
</svg>

<svg width="100" height="100">
  <image xlink:href="https://www.w3.org/TR/SVG/images/painting/fill01.svg" x="0" y="0" width="100" height="100" preserveAspectRatio="none" />
</svg>

<svg width="100" height="100">
  <image xlink:href="https://www.w3.org/TR/SVG/images/painting/fill01.svg" x="0" y="0" width="100" height="100" preserveAspectRatio="xMinYMin meet" />
</svg>

<svg width="100" height="100">
  <defs>
    <circle id="circle" cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
  </defs>
  <use xlink:href="#circle" />
</svg>
```

## Symbol

```html
<svg width="100" height="100">
  <defs>
    <symbol id="circle" viewBox="0 0 100 100">
      <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
    </symbol>
  </defs>
  <use xlink:href="#circle" />
</svg>
```

## Gradient

```html
<svg width="100" height="100">
  <defs>
    <linearGradient id="gradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <rect x="0" y="0" width="100" height="100" fill="url(#gradient)" />
</svg>
```

## Pattern

```html
<svg width="100" height="100">
  <defs>
    <pattern id="pattern" x="0" y="0" width="100" height="100" patternUnits="userSpaceOnUse">
      <rect x="0" y="0" width="100" height="100" fill="yellow" />
      <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
    </pattern>
  </defs>
  <rect x="0" y="0" width="100" height="100" fill="url(#pattern)" />
</svg>
```

## Clip Path

```html
<svg width="100" height="100">
  <defs>
    <clipPath id="clip">
      <circle cx="50" cy="50" r="40" />
    </clipPath>
  </defs>
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" clip-path="url(#clip)" />
</svg>
```

## Mask

```html
<svg width="100" height="100">
  <defs>
    <mask id="mask">
      <circle cx="50" cy="50" r="40" fill="white" />
    </mask>
  </defs>
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" mask="url(#mask)" />
</svg>
```

## Filter

```html
<svg width="100" height="100">
  <defs>
    <filter id="filter">
      <feGaussianBlur in="SourceGraphic" stdDeviation="10" />
    </filter>
  </defs>
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" filter="url(#filter)" />
</svg>

## Animation

```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow">
    <animate attributeName="cx" from="50" to="150" dur="1s" begin="0s" repeatCount="indefinite" />
  </circle>
</svg>

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow">
    <animate attributeName="cx" from="50" to="150" dur="1s" begin="0s" repeatCount="indefinite" />
    <animate attributeName="cy" from="50" to="150" dur="1s" begin="0s" repeatCount="indefinite" />
  </circle>
</svg>
```
