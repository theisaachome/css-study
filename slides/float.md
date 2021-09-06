## CSS Layout - float and clear

### Float
- Specifies how an element should float.

### Clear
- Specifies what elements can float beside the cleared element and on which side.


### The float Property
- The float property is used for positioning and formatting content 
- The avaiable values:
  - left - The element floats to the left of its container
  - right - The element floats to the right of its container
  - none - The element does not float .This is default.
  - inherit - The element inherits the float value of its parent

---

### Float right

```css
img {
  float: right;
}
```

---
### Float left

```css
img {
  float: left;
}
```

### Float Next To Each Other

```css
div {
  float: left;
  padding: 15px;
}
.div1 {
  background: red;
}
.div2 {
  background: yellow;
}
.div3 {
  background: green;
}
```

---
## CSS Layout - clear and clearfix

### The clear Property
- Specifies what should happen with the element that is next to a floating element.

- Can have one of the following values:

  - none - The element is not pushed below left or right floated elements.This is default.
  - left - The element is pushed below left floated elements
  - right - The element is pushed below right floated elements
  - both - The element is pushed below both left and right floated elements
  - inherit - The element inherits the clear value from its parent

```css
div1 {
  float: left;
}
div2 {
  clear: left;
}
```

---
### The clearfix Hack
- If a floated element is taller than the containing element, it will "overflow" outside of its container. 
- We can then add a clearfix hack to solve this problem:

```css
.clearfix {
  overflow: auto;
}
```

### modern way of clearfix
```css
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
```