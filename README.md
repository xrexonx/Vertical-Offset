# Vertical offset
Dynamic value for margin-top and margin-bottom. ~ Sass tips.

### _mtb.scss

```scss

@for $i from 0 through 100 {
  .mt-#{$i} {
    margin-top: #{$i}px;
  }

  .mb-#{$i} {
    margin-bottom: #{$i}px;
  }
}

// ~ rexon
```

### Usage 
Import this file on your app.scss

```scss
//app.scss

@import "mtb";

//another scss code here...
```

### Sample Usage on any `class` attribute

```html
<div class="mt-x mb-x"></div>

<p class="mt-30 mb-10"></p>

```
##### ~ .mt-x and .mb-x
Where: x is the value from 0 to 100, you can increment 100 to what value you want (just edit the _mtb.scss file).
