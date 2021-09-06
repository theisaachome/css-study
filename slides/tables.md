## CSS Tables

- [Table Borders](#table-borders)
- [Table Size](#table-size)
- [Table Alignment](#table-alignment)
- [Table Style](#table-style)
- [Responsive Table](#responsive-table)

---

### Table Borders
- Use the `border` property.

```css
table,th,td{
  border:1px solid black
}
```
### Full-Width Table
- Use `width` property on table element.
```css
table {
  width: 100%;
}
```
### Collapse Table Borders
- The `border-collapse` property sets the table borders should be collapsed into a single border:

```css
table {
  border-collapse: collapse;
}
```

- set border around the table
```css
table {
  border: 1px solid black;
}
```

---
###  Table Size

- Table Width and Height
- Use the width and height properties for table size.

  ```css
  table {
    width: 100%;
  }
  th {
    height: 70px;
  }
  ```

  ---

### Table Alignment
### Horizontal Alignment
  -  `text-align` property sets the horizontal alignment  of the content in `<th> or <td>`.

```css
td {
  text-align: center;
}
th {
  text-align: left;
}
```
### Vertical Alignment
-  `vertical-align` property sets the vertical alignment of the content in `<th> or <td>`.

```css
td {
  height: 50px;
  vertical-align: bottom;
}
```

--- 
### Table Style
### Table Padding
- Set the space between the border and the content in a table,
- use the padding property on `<td> and <th>` elements:

  ```css
  th, td {
    padding: 15px;
    text-align: left;
  }
  ```

### Horizontal Dividers
- Add the `border-bottom` property to <th> and <td> for horizontal dividers:
  ```css
  th, td {
    border-bottom: 1px solid #ddd;
  }
  ```

### Hoverable Table
- Use the :hover selector on `<tr>` to highlight table rows on mouse over:

  ```css
  tr:hover {background-color: yellow;}
  ```

### Striped Tables
- For zebra-striped tables,
  - Use the `nth-child()` selector
  - Add a background-color to all even (or odd) table rows:
  ```css
  tr:nth-child(even) {background-color: #f2f2f2;}
  ```

### Table Color
- Setting the background color and text color of `<th>` elements:

```css
th {
  background-color: #04AA6D;
  color: white;
}
```

---
### Responsive Table
- To make it responsive: 
  - Add a container element (like `<div>`) with overflow-x:auto around the <table> element 

```css
  <div style="overflow-x:auto;">

  <table>
  ... table content ...
  </table>

  </div>
```