## CSS Layout - The position Propertys

- Specifies the type of positioning method used for an element:
  - static, 
  - relative, 
  - fixed, 
  - absolute 
  - sticky
- Elements are then positioned using
  - top, 
  - bottom, 
  - left, and 
  - right properties.
- To work with these properties the `position` property must be  set first.
- They also work differently depending on the position value.

### `position: static`
- elements are positioned static by default.

### `position: relative`;
- Position relative to its normal position.
- Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position.
- Other content will not be adjusted to fit into any gap left by the element.
```css
div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
```

### position: fixed

- Position relative to the viewport,
- Always stays in the same place even if the page is scrolled. 
- The top, right, bottom, and left properties are used to position the element.

-  Does not leave a gap in the page where it would normally have been located.

```css
div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
```
---
### position: absolute;

- Position relative to the nearest positioned ancestor.

- If  no positioned ancestors, it uses the document body, and moves along with page scrolling.

- **Note:** 
  - Absolute positioned elements are removed from the normal flow, and can overlap elements.

  ```css
  div.relative {
    position: relative;
    width: 400px;
    height: 200px;
    border: 3px solid #73AD21;
  }

  div.absolute {
    position: absolute;
    top: 80px;
    right: 0;
    width: 200px;
    height: 100px;
    border: 3px solid #73AD21;
  }
  ```

---
### position: sticky;

- Position based on the user's scroll position.

- A sticky element toggles between relative and fixed, depending on the scroll position.
- It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed)

```css
div.sticky {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
  background-color: green;
  border: 2px solid #4CAF50;
}
```

### Overlapping Elements
- When elements are positioned, they can overlap other elements.
- The z-index property specifies the stack order of an element 
  - which element should be placed in front of, or behind, the others

### Example
- Because the image has a z-index of -1, it will be placed behind the text.
```css
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
```

### Positioning Text In an Image

```css
.container {
  position: relative;
}

.center {
  position: absolute;
  top: 50%;
  width: 100%;
  text-align: center;
  font-size: 18px;
}
.topleft {
  position: absolute;
  top: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
```