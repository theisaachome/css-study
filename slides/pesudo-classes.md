## **CSS Pseudo-classes**

- To define a special state of an element.
  - Style an element when a user mouses over it
  - Style visited and unvisited links differently
  - Style an element when it gets focus

### Syntax

- The syntax of pseudo-classes:

  ```css
  selector:pseudo-class {
    property: value;
  }
  ```

### Anchor Pseudo-classes
- Links can be displayed in different ways:


```css
/* unvisited link */
a:link {
  color: #FF0000;
}
/* visited link */
a:visited {
  color: #00FF00;
}
/* mouse over link */
a:hover {
  color: #FF00FF;
}
/* selected link */
a:active {
  color: #0000FF;
}
```

### Pseudo-classes and CSS Classes
- Pseudo-classes can be combined with CSS classes

  ```css
  a.highlight:hover {
    color: #ff0000;
  }
  ```

### Simple Tooltip Hover
- Hover over a <div> element to show a `<p>` element (like a tooltip):

```css
p {
  display: none;
  background-color: yellow;
  padding: 20px;
}
div:hover p {
  display: block;
}
```

### The :first-child Pseudo-class
- `:first-child` pseudo-class 
- Matches a specified element that is the first child of another element.
- matches any `<p>` element that is the first child of any element:

  ```css
  p:first-child {
    color: blue;
  }
  ```
- Matches the first `<i>` element in all `<p>` elements:
  ```css
  p i:first-child {
    color: blue;
  }
  ```

- Matches all `<i>` elements in `<p>` elements that are the first child of another element:
  ```css
  p:first-child i {
    color: blue;
  }
  ```
