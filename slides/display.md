## The display Property


- The display property is the most important CSS property for controlling layout.

### The display Property
- The display property specifies if/how an element is displayed.

### Block-level Elements
- always starts on a new line and takes up the full width available 

- Examples of block-level elements:
  - div
  - h1 - h6
  - p
  - form
  - header
  - footer
  - section
### Inline Elements
- only takes up as much width as necessary.
- Examples of inline elements:
  - span
  - a
  - img

---

### Display: none
- `display: none;` 
- to hide and show elements without deleting and recreating them.

### Override The Default Display Value
-  inline `<li>` elements for horizontal menus:
  ```css
  li {
    display:inline;
  }
  ```
- displays `<span>` elements as block elements:
  ```css
  span {
    display: block;
  }
  ```
- displays `<a>` elements as block elements:
  ```css
  a {
    display: block;
  }
  ```

---
### Hide an Element

### display:none 
- The `display:none` property to  hide an element .
- The page will be displayed as if the element is not there:

  ```css
  h1.hidden {
    display: none;
  }
  ```
###  visibility:hidden
- `visibility:hidden` also hides an element.
- The element will be hidden, but still affect the layout:

  ```css
  h1.hidden {
    visibility: hidden;
  }
  ```