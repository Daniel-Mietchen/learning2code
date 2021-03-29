# About

Some notes regarding HTML and HTML5.

# Resources

* FreeCodeCamp: [Introduction to Basic HTML & HTML5](https://www.freecodecamp.org/learn/responsive-web-design/basic-html-and-html5/)
* W3C Schools: [HTML tutorial](https://www.w3schools.com/html/)

# Examples
* the ```target="_blank"``` attribute on an HTML element triggers the linked document to be opened in a new browser tab.
* to create a form field for text input, use ```<input type="text" placeholder="sample text">``` 
* to make a form field required, use ```required``` after the type attribute of the input element: ```<input type="text" required placeholder="sample text">```
* to create radio buttons, use ```<input id="buttongroupid" type="radio" name="sample-radio-buttons">```
  - to assist assistive technologies, it is recommended to add a ``for``` tag, as in 
  ```HTML
  <label for="buttongroupid">   
    <input id="buttongroupid" type="radio" name="sample-radio-buttons">Indoor 
  </label>
  ```
* to submit form content to a server, use ```<form action="https://example.org/form-processing"><input type="text" placeholder="sample text"></form>```
* to create a button for form submission, use a ```button``` attribute: ```<form action="https://example.org/form-processing"><input type="text" placeholder="sample text"><button type="submit">Submit</button></form>```

# Testing grounds

* [NurKurz.Online](https://nurkurz.online/)
* [CodeGround](https://www.codeground.org/)
