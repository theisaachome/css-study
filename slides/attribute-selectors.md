## **CSS Attribute Selectors**

- To select elements with a specified attribute.


  ```css
  a[target] {
    background-color: yellow;
  }
  ```

### CSS [attribute="value"] Selector

- To select elements with a specified attribute and value.
  ```css
  a[target="_blank"] {
    background-color: yellow;
  }
  ```

### CSS [attribute~="value"] Selector
- To select elements with an attribute value containing a specified word.

  ```css
  [title~="flower"] {
    border: 5px solid yellow;
  }
  ```

### CSS [attribute|="value"] Selector

- To select elements with the specified attribute starting with the specified value.
- **Note:** The value has to be a whole word, either alone,
  - like `class="top"`, or
  - followed by a `hyphen( - )`,
  - like `class="top-text"`! 
  ```css
  [class|="top"] {
    background: yellow;
  }
  ```


### **CSS [attribute^="value"] Selector**

-  To select elements whose attribute value begins with a specified value.
- Note: The value does not have to be a whole word! 
  ```css
  [class^="top"] {
    background: yellow;
  }
  ```

### CSS [attribute$="value"] Selector
- To select elements whose attribute value ends with a specified value.
- Note: The value does not have to be a whole word!  
  ```css
  [class$="test"] {
    background: yellow;
  }
  ```

### CSS [attribute*="value"] Selector
- To select elements whose attribute value contains a specified value.
-  Note: The value does not have to be a whole word!  

  ```css
  [class*="te"] {
    background: yellow;
  }
  ```