# SASS Variables



A variable declaration looks a lot like a property declaration: it’s written   
`<variable>: <expression>`.

```scss
$base-color: #c6538c;
$border-dark: rgba($base-color, 0.88);

.alert {
  border: 1px solid $border-dark;
}
```


```scss
$font-weights:(
    "regular":400,
    "medium":500,
    "bold":700
)

body{
    font-weight: map-get($font-weights , bold );
}

```