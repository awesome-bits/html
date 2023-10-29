# Math

The <math> MathML element is the top-level MathML element, used to write a single mathematical formula. It can be placed in HTML content where flow content is permitted.

```html
<math display="inline">
</math>

<math display="block">
</math>
```

```html
<math>
  <mrow>
    <mi>a</mi>
    <mo>+</mo>
    <mi>b</mi>
    <mo>=</mo>
    <mn>5</mn>
  </mrow>
</math>
```

```html
<math display="block">
  <mrow>
    <munderover>
      <mo>∑</mo>
      <mrow>
        <mi>n</mi>
        <mo>=</mo>
        <mn>1</mn>
      </mrow>
      <mrow>
        <mo>+</mo>
        <mn>∞</mn>
      </mrow>
    </munderover>
    <mfrac>
      <mn>1</mn>
      <msup>
        <mi>n</mi>
        <mn>2</mn>
      </msup>
    </mfrac>
  </mrow>
</math>
```
  
```html
this is real number: 
<math display="inline">
  <mfrac>
    <msup>
      <mi>π</mi>
      <mn>2</mn>
    </msup>
    <mn>6</mn>
  </mfrac>
</math>
```