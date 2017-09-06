*This fork drops classes, replacing them with [placeholders](http://sass-lang.com/documentation/Sass/Selector/Placeholder.html).*

# Angled Edges (SASS mixin)

[Live demo](http://nigelotoole.github.io/angled-edges/)

Add a consistent angled edge to a full width element. This technique uses CSS [clip-path](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path) to clip the image but has a fallback using pseudo elements for [older browsers](http://caniuse.com/#feat=css-clip-path). It is only intended for use on full width elements as it uses the `vw` unit to calculate the angle.


## Usage

Once you have downloaded the code, run the commands below to view the demo.

```javascript
$ npm install
$ gulp serve
```

You can also import **angled-edges.scss** into your own project directly and use the classes already setup or use the mixin in your own classes.


Follow the code example below for basic usage with an angle on the top left.

```scss
@import "angled-edges.scss";

.angle--top-left {
  @extend %angle--top-left;
}
```

```html
<div class="angle--top-left">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/Sig07-007.jpg/1280px-Sig07-007.jpg" alt="Nebula" class="angle__content">
</div>
```


### License
MIT © Nigel O Toole
