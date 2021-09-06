## **CSS Layout - Overflow**

- Controls what happens to content that is too big to fit into an area.

- The overflow property has the following values:

  - `visible: ` Default. The overflow is not clipped. The content renders outside the element's box
  - `hidden: ` The overflow is clipped, and the rest of the content will be invisible
  - `scroll: ` The overflow is clipped, and a scrollbar is added to see the rest of the content
  - `auto: ` Similar to scroll, but it adds scrollbars only when necessary

- only works for block elements with a specified height.

### **overflow: visible**

```css
div {
  width: 200px;
  height: 50px;
  background-color: #eee;
  overflow: visible;
}
```

### overflow: hidden
- With the `hidden` value, the overflow is clipped, and the rest of the content is `hidden`:

```css
.hidden {
  overflow: hidden;
}
```

### overflow: scroll
- Setting the value to `scroll`, the overflow is clipped and a scrollbar is added to scroll inside the box.
- **Note** both horizontally and vertically scrollbar

```css
.scroll {
  overflow: scroll;
}
```

### overflow: auto
- The `auto` value is similar to scroll, but it adds scrollbars only when necessary:

```css
.auto {
  overflow: auto;
}
```


### overflow-x and overflow-y
- The overflow-x and overflow-y properties specifies whether to change the overflow of content just horizontally or vertically (or both):

  - overflow-x specifies what to do with the left/right edges of the content.
  - overflow-y specifies what to do with the top/bottom edges of the content.
```css
.x-and-y-scroll {
  overflow-x: hidden; /* Hide horizontal scrollbar */
  overflow-y: scroll; /* Add vertical scrollbar */
}
```