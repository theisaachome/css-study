### CSS Combinators
- A CSS selector can contain more than one simple selector.
- A combinator is something that explains the relationship between the selectors.

- There are four different combinators in CSS:
  - descendant selector (space)
  - child selector (>)
  - adjacent sibling selector (+)
  - general sibling selector (~)

### Descendant Selector
- Matches all elements that are descendants of a specified element.

- selects all `<p>` elements inside `<div>` elements: 

```css
div p {
  background-color: yellow;
}
```

### Child Selector (>)
-  Selects all elements that are the children of a specified element.

-  selects all `<p>` elements that are children of a `<div>` element:
```css
div > p {
  background-color: yellow;
}
```

### Adjacent Sibling Selector (+)

- select an element that is directly after another specific element.
- `Sibling` elements must have `the same parent element`
- `adjacent` means `immediately following`.
- selects the first p element that are placed immediately after div elements:
``` css
div + p {
  background-color: yellow;
}
```

### General Sibling Selector (~)

- Selects all elements that are next siblings of a specified element.

- Selects all `<p>` elements that are next siblings of `<div>` elements: 


```css
div ~ p {
  background-color: yellow;
}
```