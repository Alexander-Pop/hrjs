# HR.js

> Tiny JavaScript plugin for highlighting and replacing text in the DOM



## Install

Include hr.js file
```html
<script src="src/hr.js"></script>
```
or use CDN
```html
<script src="https://rawgit.com/mburakerman/hrjs/master/src/hr.js"></script>
```



## Usage

```html
 <p id="mytext">Lorem ipsum dolor sit amet.</p>
```
Activate

```js
<script>
   new HR("#mytext", {
     highlight: "dolor",
     replaceWith: "cat",
     backgroundColor: "#B4FFEB"
   }).hr();
</script>
```
Thats it!

[CodePen demo](https://codepen.io/anon/pen/ZKWBYV)

![CodePen demo](https://media.giphy.com/media/l4FGuX1VuJFbENUjK/giphy.gif)


## Multiple

You can also highlight and replace multiple keywords.

```html
 <p id="mytext">I love JavaScript.</p>
```

```js
<script>
   new HR("#mytext", {
     highlight: ["love","JavaScript"],
     replaceWith: ["like", "jQuery"],
     backgroundColor: "#B4FFEB"
   }).hr();
</script>
```
[CodePen demo](https://codepen.io/anon/pen/XRdNbw)



### Highlight example

To highlight only, just add your keyword to `highlight` option.

```html
 <p class="mytext">Lorem ipsum dolor sit consectetur amet.</p>
 <h3 class="mytext">Consectetur enim ipsam voluptatem quia</h3>
```

```js
<script>
  new HR(".mytext", {
    highlight: "consectetur",
    backgroundColor:"#B4FFEB"
  }).hr();
</script>
```
[CodePen Highlight demo](https://codepen.io/anon/pen/Vbampm)



## Customize

These are default options.

```js
  new HR("elem", {
    highlight:null,
    replaceWith: null,
    backgroundColor:"#FFDE70"
  }).hr();
```



## License

Licensed under the MIT License.
