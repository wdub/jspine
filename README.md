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

<h3>Attributes</h3>
* text          - set the text contents or get the text content of matched elements
* html          - set the HTML contents or get the HTML content of an element
* hasClass      - check whether any of the matched elements are assigned the given class
* addClass      - adds one or more classes
* removeClass   - remove one or more classes
* toggleClass   - adds or remove the specified class
* attr          - get the value of an attribute or set an attribute
* append        - insert a new element at the end
* prepend       - insert a new element at the beginning
* toggle        - show or hide an element
* isVisible     - check if an element is visible
* show          - display an element
* hide          - hide an element
* remove        - remove one or more elements
* newel         - create a new element
* empty         - remove all child nodes
* loader        - display or hide an animation(GIF or CSS keyframes required)
* message       - display or hide a custom message
* data          - get or set data attribute value
* on            - attach an event handler function to one or more elements
* off           - remove an event handler
* xobj          - returns the XmlHttpRequest Object so it can be used for file uploads or other purposes
* xhr           - perform an asynchronous HTTP request
* formData      - encode and return a set of form elements

<h3>Demo</h3>
[jSpine examples](http://jspine.techlabs.ro/)
