## **CSS Layout - Horizontal & Vertical Align**

### Center Align Elements

- To horizontally center a block element (like `<div>`),
- use `margin: auto`;
```css
.center {
  margin: auto;
  width: 50%;
  border: 3px solid green;
  padding: 10px;
}
```

### Center Align Text
- To just center the text inside an element, use text-align: center;
```css
.center {
  text-align: center;
  border: 3px solid green;
}
```

### Center an Image
- To center an image, set left and right margin to auto and make it into a block element:
```css
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 40%;
}
```

### Left and Right Align - Using position
One method for aligning elements is to use position: absolute;
```css
.right {
  position: absolute;
  right: 0px;
  width: 300px;
  border: 3px solid #73AD21;
  padding: 10px;
}
```

### Left and Right Align - Using float
- Another method for aligning elements is to use the float property:
```css
.right {
  float: right;
  width: 300px;
  border: 3px solid #73AD21;
  padding: 10px;
}
```

### Center Vertically - Using padding
- A simple solution is to use top and bottom padding:
```css
.center {
  padding: 70px 0;
  border: 3px solid green;
}
.center {
  padding: 70px 0;
  border: 3px solid green;
  text-align: center;
}
```