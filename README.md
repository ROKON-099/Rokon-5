1.What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?

2. How do you **create and insert a new element into the DOM**?

3. What is **Event Bubbling** and how does it work?

4. What is **Event Delegation** in JavaScript? Why is it useful?

5.  What is the difference between **preventDefault() and stopPropagation()** methods?
  ---------------------------------------------------------------------------------
  
  --------------------------------------------------------------------------------

Answer to the question no.1:

Difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll :

getelementbyid: getElementById is a JavaScript method that selects a single HTML element by its unique id and returns the element, or null if not found.
We can use it on ,To select a specific HTML element using its unique id.

getelementbyclass: getElementsByClassName is a JavaScript method used to select all HTML elements that have a specific class name.
The main reason to use getelementbyclass is we can select multiple element by it .

querySelector and querySelectorAll : querySelector and querySelectorAll are JavaScript methods used to select HTML elements using CSS selectors. But there are little difference between querySector and querySelectorAll,

querySelector: It  Selects the first element that matches a CSS selector.
And return A single element.
On the other hand,

querySelectorAll: It select the all element that a matches a CSS selector.
And it return a nodelist.


----------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------

Answer to the question no.2:

I create  and insert a new element into the DOM by using some step those are 

1.At first create a new element.

2.Then add content or attributes.

3. Select the parent element.

4.Insert the new element into the DOM.

Example:
<!--html-->
<div id="container"></div>

< --js-->
const newDiv = document.createElement("div");

//add content

newDiv.textContent = "Hello World";

// Insert into container

document.getElementById("container").appendChild(newDiv);


--------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------


Answer to the question no.3:

Event Bubbling is when an event starts at the target element and propagates upward through its parent elements in the DOM.

The working process of it ;

1.	Event occurs on the target element (the element you clicked).

2.	Event triggers the target’s event handler first.

3.	Event moves up to the parent element, triggering its event handler.

4.	Event continues to bubble up through all ancestor elements up to <html>.

5.	Bubbling can be stopped using event.stopPropagation().

   --------------------------------------------------------------------
   -------------------------------------------------------------------

   Answer to the question no .4:
   
Event Delegation is a JavaScript technique where a single event listener is attached to a parent element to handle events for its child elements, instead of attaching separate listeners to each child.

It is very usefull because of some reason that are;

1.	It improves performance

2.It can handles dynamic elements
    
3. Very Simpler to code
	 
4.Leverages event bubbling
	
5. Scalable .


_________________________________________________________________________________________________
_________________________________________________________________________________________________


Answer to the question no.5

Difference between **preventDefault() and stopPropagation() are 

preventDefault() is a JavaScript method that stops the default action of an element, such as preventing a link from navigating to a URL or stopping a form from submitting. However, it does not affect the event’s propagation through the DOM.

 On the other hand, stopPropagation() prevents the event from bubbling up (or capturing down) the DOM tree, so parent elements do not receive the event, but it does not stop the element’s default action. Essentially, preventDefault() controls what the element does by default, while stopPropagation() controls how the event moves through the DOM.


















			
			
			


