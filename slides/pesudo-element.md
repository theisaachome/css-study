## **CSS Pseudo-elements**

- To style specified parts of an element.
- It can be used to:
  - Style the first letter, or line, of an element
  - Insert content before, or after, the content of an element

### Syntax
- The syntax of pseudo-elements:

```css 
selector::pseudo-element {
  property: value;
}
```

### The ::first-line Pseudo-element
- Add a special style to the first line of a text.

- formats the first line of the text in all `<p>` elements:

```css
p::first-line {
  color: #ff0000;
  font-variant: small-caps;
}
```
### The ::first-letter Pseudo-element

- Add a special style to the first letter of a text.
- Formats the first letter of the text in all `<p>`elements: 
```css
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}
```

### Multiple Pseudo-elements

- Several pseudo-elements can also be combined.

  ```css
  p::first-letter {
    color: #ff0000;
    font-size: xx-large;
  }

  p::first-line {
    color: #0000ff;
    font-variant: small-caps;
  }
  ```
### CSS - The ::before Pseudo-element
- used to insert some content before the content of an element.
- inserts an image before the content of each <h1> element:

  ```css
  h1::before {
    content: url(smiley.gif);
  }
  ```

### CSS - The ::after Pseudo-element
- used to insert some content after the content of an element.
- inserts an image after the content of each `<h1> `element:

  ```css
  h1::after {
    content: url(smiley.gif);
  }
  ```


### CSS - The ::marker Pseudo-element

- The ::marker pseudo-element selects the markers of list items.
- Styles the markers of list items:

  ```css
  ::marker {
    color: red;
    font-size: 23px;
  }
  ```
### CSS - The ::selection Pseudo-element

- The `::selection` matches the portion of an element that is selected by a user.
- The following CSS properties can be applied to ::selection: color, background, cursor, and outline.

- The selected text red on a yellow background:

```css
::selection {
  color: red;
  background: yellow;
}
```