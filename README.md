# scss-aspect-ratio

## overview

Simple SCSS Aspect Ratios.

## installation

npm install --save scss-aspect-ratio

## usage

```scss

@import "scss-aspect-ratio/scss-aspect-ratio";

.ratio-16-9 {
  @include aspect-ratio(16,9); // creates an element that is 16x9
  .content{
    position: absolute;
    width: 100%;
    height: 100%;
  }
}

```

## output

```scss

  .ratio-16-9 {
    position: relative;
  }
  .ratio-16-9:before {
    content: "";
    display: block;
    width: 100%;
    padding-top: 56.25%;
  }
  .ratio-16-9 .content{
    position: absolute;
    width: 100%;
    height: 100%;
  }
}

```
