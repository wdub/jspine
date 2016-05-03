<h1>jSpine v1.3.3</h1>
Yet another fast and lightweight Javascript library.

<h3>Usage</h3>
<h5>DOM objects manipulation</h5>
```html
<div class="test" style="display:none"></div>
```
```javascript
function(){
  var testDiv = $('.test');
  testDiv.text('Content...').show();
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
<h5>Event delegation</h5>
```html
<ul class="container">
    <li class="l1">L1</li>
    <li class="l2">
        <span>Title 1</span>
    </li>
    <li class="l3">
        <div>
            <strong id="title">Title 2</strong>
            <p class="sub sub1">Subtitle 1</p>
            <p class="sub sub2">Subtitle 2</p>
        </div>
    </li>
    <li class="l4">L4</li>
</ul>
```
```javascript
$('.container').on('click', '.sub', function (ev, clicked) {
    ev.preventDefault();
    $(clicked).hide();
});
```

<h5>XMLHttpRequest</h5>
```html
<button class="xhr-btn">Get response</button>
<p class="response"></p>
```
```javascript
$('.xhr-btn').on('click', function (e) {
  $().xhr('param=demo', './json.php', function (response) {
    $('.response').text(response);
  })
});
```

### Attributes
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
