Images
====

## SVG as `<img>`

Where possible we should look to use SVG in our builds.

It's important however, to provide a fallback solution often in the shape of a PNG replacement.

Firstly we need to test for support of SVG images as inline elements.

If we're using Modernizr this can be done using the following test function
```
Modernizr.addTest('svgasimg', document.implementation.hasFeature('http://www.w3.org/TR/SVG11/feature#Image', '1.1'));
```

Note: The default Modernizr SVG test only tests for SVG as `<embed>` or `<object>` but should be updating soon. See [CSS-Tricks "Test for Support of SVG as img"](http://css-tricks.com/test-support-svg-img/).