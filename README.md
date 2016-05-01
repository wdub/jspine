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
* __text__          - set the text contents or get the text content of matched elements
* __html__          - set the HTML contents or get the HTML content of an element
* __hasClass__      - check whether any of the matched elements are assigned the given class
* __addClass__      - adds one or more classes
* __removeClass__   - remove one or more classes
* __toggleClass__   - adds or remove the specified class
* __attr__          - get the value of an attribute or set an attribute
* __append__        - insert a new element at the end
* __prepend__       - insert a new element at the beginning
* __toggle__        - show or hide an element
* __isVisible__     - check if an element is visible
* __show__          - display an element
* __hide__          - hide an element
* __remove__        - remove one or more elements
* __newel__         - create a new element
* __empty__         - remove all child nodes
* __loader__        - display or hide an animation(GIF or CSS keyframes required)
* __message__       - display or hide a custom message
* __data__          - get or set data attribute value
* __on__            - attach an event handler function to one or more elements
* __off__           - remove an event handler
* __xobj__          - returns the XmlHttpRequest Object so it can be used for file uploads or other purposes
* __xhr__           - perform an asynchronous HTTP request
* __formData__      - encode and return a set of form elements

<h3>Demo</h3>
[jSpine examples](http://jspine.techlabs.ro/)
