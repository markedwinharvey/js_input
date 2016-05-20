<h4>js_input</h4>

Customizable prompt-style javascript module for getting basic user input. 

![js_input_box](https://github.com/markedwinharvey/js_input/blob/master/media/js_input_graphic.png)

js_input.js can be loaded in a script tag and invoked with a function call js_input(dict) where
dict is a dictionary/object featuring key:value data pairs. 
<br>
The pairs may include:
	<br>
	input_msg:	message to display in prompt to user
	<br>
	el:			js_input_box gets appended to this element; js_input_box becomes first child of <body> if el is unspecified
	<br>
	callback:	callback function to execute on completion of prompt
	<br>
	params:		js object of key:value pairs passed as parameter list in callback function
	
A simple, customizable html template for the prompt (#js_input_box) is embedded in the javascript. 

When js_input(dict) is called, the input box is appended to the html document. 
<br>
The prompt collects user input, adds this input to dict.params, 
executes the callback function (passing params object),
and removes itself from the document. 