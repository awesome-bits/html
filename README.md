# Table

The elements here are used to create and handle tabular data.

```html
<table>
</table>
```

## Table Caption

Table caption is used to provide a title for a table.

```html
<table>
  <caption>This is caption of table</caption>
</table>
```

## Table Body

Table body is used to group the body content in a table.

```html
<table>
  <tbody>
  </tbody>
</table>
```

## Table Row

Table row is used to group the table cells in a table.

```html
<table>
  <tbody>
    <tr>
      this is row
    </tr>
  </tbody>
</table>
```

## Table Data

Table Data is used to group the table cells in a table.

```html
<table>
  <tbody>
    <tr>
      <td>Column 1</td>
      <td>Column 2</td>
    </tr>
  </tbody>
</table>
```

## Table Header

Table header is used to group the header content in a table.

```html
<table>
  <thead>
    <tr>
      this is head
    </tr>
  </thead>
</table>
```

## Table row header

Table row header is used to group the header content in a table.

```html
<table>
  <thead>
    <tr>
      <th>Column 1</th>
      <th>Column 2</th>
    </tr>
  </thead>
</table>
```

## Table Footer

Table footer is used to group the footer content in a table.

```html
<table>
  <tfoot>
    <tr>
      <td>Column 1</td>
      <td>Column 2</td>
    </tr>
  </tfoot>
</table>
```

## Column Group

Colgroup is used to group the columns in a table.

```html
<table>
  <colgroup>
  </colgroup>
</table>
```

## Column

Col is used to define the width and other attributes for each column.

```html
<table>
  <caption>
    Superheros and sidekicks
  </caption>
  <colgroup>
    <col />
    <col span="2" />
    <col span="2" />
  </colgroup>
  <tr>
    <td> </td>
    <th scope="col">Batman</th>
    <th scope="col">Robin</th>
    <th scope="col">The Flash</th>
    <th scope="col">Kid Flash</th>
  </tr>
  <tr>
    <th scope="row">Skill</th>
    <td>Smarts</td>
    <td>Dex, acrobat</td>
    <td>Super speed</td>
    <td>Super speed</td>
  </tr>
</table>
```

## Table Example

```html
<table border="1">
  <caption>
    Superheros and sidekicks
  </caption>
  <colgroup>
    <col />
    <col span="2" />
    <col span="2" />
  </colgroup>
  <thead>
    <tr>
      <td> </td>
      <th scope="col">Batman</th>
      <th scope="col">Robin</th>
      <th scope="col">The Flash</th>
      <th scope="col">Kid Flash</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Skill</th>
      <td>Smarts</td>
      <td>Dex, acrobat</td>
      <td>Super speed</td>
      <td>Super speed</td>
    </tr>
    <tr>
      <th scope="row">Skill</th>
      <td>Smarts</td>
      <td>Dex, acrobat</td>
      <td>Super speed</td>
      <td>Super speed</td>
    </tr>
    <tr>
      <th scope="row">Skill</th>
      <td>Smarts</td>
      <td>Dex, acrobat</td>
      <td>Super speed</td>
      <td>Super speed</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td> </td>
      <th scope="col">Batman</th>
      <th scope="col">Robin</th>
      <th scope="col">The Flash</th>
      <th scope="col">Kid Flash</th>
    </tr>
  </tfoot>
</table>
```