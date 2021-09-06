##  CSS Lists

- Specifies the type of list item marker.
- The available list item:
    - circle
    - square
    - upper-roman
    - lower-alpha
  ```css
  ul.a {
    list-style-type: circle;
  }
  ```
- Specifies an image as the list item marker.
  ```css
  ul {
    list-style-image: url('sqpurple.gif');
  }
  ```
## Position

-  Specifies the position of the list-item markers. 
    ```css
      ul.a {
        list-style-position: outside;
      }
      ul.b {
        list-style-position: inside;
      }
    ```