# Vertical offset
Dynamic value for margin-top and margin-bottom. ~ Sass tips.

### _mtmb.scss

```scss

@for $i from 0 through 100 {
  .mt-#{$i} {
    margin-top: #{$i}px;
  }

  .mb-#{$i} {
    margin-bottom: #{$i}px;
  }
  
  .mt-mb-#{$i} {
    margin-top: #{$i}px;
    margin-bottom: #{$i}px;
  }
}

// ~ rexon
```

### Usage 
Import this file on your app.scss

```scss
//app.scss

@import "mtmb";

//another scss code here...
```

### Sample Usage on any `class` attribute

```html
<div class="mt-x mb-x"></div>

<p class="mt-30 mb-10"></p>

<!-- If both have the same value like this -->
<div class="mt-15 mb-15"></div>

<!-- You can simple do this -->
<div class="mt-mb-15"></div>

```
##### ~ .mt-x,.mb-x and mt-mb-x
Where: x is the value from 0 to 100, you can increment 100 to what value you want (just edit the _mtmb.scss file).
