# Form

HTML provides several elements that can be used together to create forms that the user can fill out and submit to the website or application. 

## Button

The `<button>` element represents a clickable button, which can be used in forms or anywhere in a document that needs simple, standard button functionality. By default, HTML buttons are presented in a style resembling the platform the user agent runs on, but you can change buttons’ appearance with CSS.

- onclick : The onclick attribute fires on a mouse click on the element.
- disabled : The disabled attribute is a boolean attribute. When present, it specifies that the button should be disabled.

```html
<button type="button" disabled>Click Me!</button>

<button type="button" onclick="alert('Hello world!')">Click Me!</button>

<button onclick="myFunction()">Click me</button>

<script>
  function myFunction() {
    alert("Hello World!");
  }
</script>
```

## Input

The `<input>` element is the most important form element. The `<input>` element can be displayed in several ways, depending on the type attribute.

- type : The type attribute specifies the type of <input> element to display.
- name : The name attribute specifies the name of an <input> element.
- value : The value attribute specifies the initial value of an <input> element.
- disabled : The disabled attribute is a boolean attribute. When present, it specifies that the <input> element should be disabled.
- readonly : The readonly attribute is a boolean attribute. When present, it specifies that an input field is read-only.

```html
<input type="text" name="firstname" value="John">

<input type="text" name="firstname" value="John" disabled>

<input type="text" name="firstname" value="John" readonly>

<input type="text" name="firstname" value="John" size="40" maxlength="50">

<input type="text" name="firstname" value="John" size="40" minlength="4">

<input type="text" name="firstname" value="John" size="40" pattern="[A-Za-z]{3}">

<input type="text" name="firstname" value="John" size="40" placeholder="John Doe">

<input type="text" name="firstname" value="John" size="40" list="browsers">

<input type="text" name="firstname" value="John" size="40" autocomplete="off">

<input type="text" name="firstname" value="John" size="40" autofocus>

<input type="text" name="firstname" value="John" size="40" required>

<input type="email" name="email" value="John" size="40" required>
```

## Label

The `<label>` element represents a caption for an item in a user interface.

- for : The for attribute specifies which form element a label is bound to.

```html
<label for="email">
  Email:
</label>
<input type="email" id="email" name="email">
``` 

## Textarea

The `<textarea>` element represents a multi-line plain-text editing control.

- cols : The cols attribute specifies the visible width of a text area.
- rows : The rows attribute specifies the visible number of lines in a text area.

```html
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```

## Select

The `<select>` element represents a control that provides a menu of options.

- name : The name attribute specifies the name of a <select> element.
- size : The size attribute specifies the number of visible options in a drop-down list.
- multiple : The multiple attribute specifies that multiple options can be selected at once.
- disabled : The disabled attribute is a boolean attribute. When present, it specifies that an option should be disabled.
- autofocus : The autofocus attribute is a boolean attribute. When present, it specifies that an option should automatically get focus when the page loads.
- required : The required attribute is a boolean attribute. When present, it specifies that an option must be selected before submitting the form.

```html
<select name="cars" size="3" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```

## Option

The `<option>` element is used to define an item contained in a `<select>`, an `<optgroup>`, or a `<datalist>` element. As such, `<option>` can represent menu items in popups and other lists of items in an HTML document.

- value : The value attribute specifies the value to be sent to a server when a form is submitted.
- disabled : The disabled attribute is a boolean attribute. When present, it specifies that an option should be disabled. 
- selected : The selected attribute is a boolean attribute. When present, it specifies that an option should be pre-selected when the page loads.

```html
<select name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab" selected>Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```

## Datalist

The `<datalist>` element contains a set of `<option>` elements that represent the permissible or recommended options available to choose from within other controls.
  
```html
<input list="browsers" name="browser">
<datalist id="browsers">
  <option value="Internet Explorer">
  <option value="Firefox">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

## Optgroup

The `<optgroup>` element creates a grouping of options within a `<select>` element.

- disabled : The disabled attribute is a boolean attribute. When present, it specifies that an option should be disabled.

```html
<select name="cars">
  <optgroup label="Swedish Cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
  </optgroup>
  <optgroup label="German Cars">
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>
```

## Form

The `<form>` element represents a document section that contains interactive controls for submitting information to a web server.

- action : The action attribute specifies where to send the form-data when a form is submitted.
- method : The method attribute specifies the HTTP method (GET or POST) to be used when submitting the form-data.
- target : The target attribute specifies a name or a keyword that indicates where to display the response that is received after submitting the form.
- autocomplete : The autocomplete attribute specifies whether a form should have autocomplete on or off.
- enctype : The enctype attribute specifies how the form-data should be encoded when submitting it to the server.
- name : The name attribute specifies the name of a form.
- novalidate : The novalidate attribute specifies that the form should not be validated when submitted.

```html
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

## Fieldset

The `<fieldset>` element is used to group several controls as well as labels (`<label>`) within a web form.

- disabled : The disabled attribute is a boolean attribute. When present, it specifies that the fieldset should be disabled.
- form : The form attribute specifies one or more forms an <fieldset> element belongs to.
- name : The name attribute specifies the name of a <fieldset> element.

```html
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

## Legend

The `<legend>` element represents a caption for the content of its parent `<fieldset>`.

```html
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset> 
</form>
```

## Meter

The `<meter>` element represents either a scalar value within a known range or a fractional value.

- value : The value attribute specifies the current value of the gauge.
- min : The min attribute specifies the minimum value of the gauge.
- max : The max attribute specifies the maximum value of the gauge.
- low : The low attribute specifies the range that is considered to be the low end of the gauge.
- high : The high attribute specifies the range that is considered to be the high end of the gauge.
- optimum : The optimum attribute specifies the range that is considered to be the optimum value of the gauge.

```html
<meter value="2" min="0" max="10">2 out of 10</meter>
```

## Progress

The `<progress>` element represents the completion progress of a task, typically displayed as a progress bar.

- value : The value attribute specifies how much of the task has been completed.
- max : The max attribute specifies how much work the task requires in total.

```html
<progress value="22" max="100">22%</progress>
```

## Output

The `<output>` element represents the result of a calculation or user action.

- for : The for attribute specifies the relationship between the result of the calculation, and the elements used in the calculation.
- form : The form attribute specifies one or more forms an <output> element belongs to.
- name : The name attribute specifies the name of a <output> element.

```html
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  <input type="range" id="a" name="a" value="50">
  +<input type="number" id="b" name="b" value="25">
  =<output name="x" for="a b"></output>
</form>
```
