Website Performance Optimization
-------------------------------------------------------------------------------
Cameron Pittman's portfolio website has been optimized

#### How to start
* Serve on localhost If you're familiar with python run these commands on your terminal

```
git clone https://github.com/Sh4reef/fend-mp.git
cd fend-mp
sudo python -m SimpleHTTPServer 80 

```

Open your browser and navigate to `http://localhost` or `http:/127.0.0.1`

* Live website
[Here](https://sh4reef.github.io/fend-mp)

#### PageSpeed score
[Here](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fsh4reef.github.io%2Ffend-mp&tab=mobile)

#### Implemented optimizations
`index.html`

- External link to `style.css` has been removed, Implemented internal `<style>` instead.
- Added `rel="dns-prefetch"` attribute `<link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="dns-prefetch">`.
- Added `media="print"` attribute `<link href="css/print.css" rel="stylesheet" media="print">`.
- Added `async` attribute `<script async src="https://www.google-analytics.com/analytics.js"></script>`.

`main.js`
- Removed `determineDx()` function.
- Refactored `changePizzaSizes()` and `updatePosition()` functions.
- Refactored DOM elements calls, And use `getElementById()`, `getElementByClassName()`.
- Moved some variable declaration outside the loop.

`pizza.html`
- Fixed the image.

`style.css` for `pizza.html`
- Added `backface-visibility: hidden;` property with `hidden` value.