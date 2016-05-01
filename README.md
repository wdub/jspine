<h1>jSpine</h1>
Yet another fast and lightweight Javascript library.

<h3>Usage</h3>
<h5>DOM objects manipulation</h5>
```html
<div class="test" style="display:none"></div>
```
```javascript
function(){
  var testDiv = $('.test');
  testDiv.text('Populate div#test').show();
  // now we can add one or more classes
  testDiv.addClass('first second');
}
```

<h5>Event handling</h5>
```html
<button class="toggle">Toggle</button>
<div class="content">
  This will be shown/hidden
</div>
```
```javascript
$('.toggle').on('click', function(e){
  e.preventDefault();
  $('.content').toggle();
}
```

<h3>Properties</h3>
* text
* html
* hasClass
* addClass
* removeClass
* toggleClass
* attr
* append
* prepend
* toggle
* isVisible
* show
* hide
* remove
* newel
* empty
* loader
* message
* data
* on
* off
* xobj
* xhr
* formData

<h3>Demo</h3>
[jSpine examples](http://jspine.techlabs.ro/)
