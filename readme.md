

1.
getElementById("id")  Finds one element by its unique id.
getElementsByClassName("class")  Finds many elements that have the same class name.
querySelector("selector")  Finds the first element that matches a CSS rule (like #id, .class, tag).
querySelectorAll("selector")  Finds all elements that match a CSS rule.

----------------------------------------------------------------------------------------------------------------------------------

2.
To create and insert a new element into the DOM, you first use document.createElement("tagName") to make the element. After creating it, you can add text, classes, or attributes, for example by setting textContent, id, or className. Finally, you place the element into the page using methods like appendChild() or prepend(). For example, if you create a <p> element, add some text to it, and then use document.body.appendChild(newPara), the new paragraph will appear at the end of the page. This way, you can dynamically add new content to your webpage.

----------------------------------------------------------------------------------------------------------------------------------


3.
Event bubbling means that when you do something (like click) on a small element, the event also goes up to its parent elements.
For example, if you click a button inside a <div>, first the button feels the click, then the <div> feels it, then the <body> feels it, and so on. The event “bubbles up” like a bubble in water, moving from the inside element to the outside elements.

----------------------------------------------------------------------------------------------------------------------------------


4.
Event delegation means putting one event listener on a parent element instead of many listeners on each child element. Because of event bubbling, when you click a child, the event goes up to the parent, and the parent can check which child was clicked.
It is useful because it makes your code simpler, faster, and works even if new child elements are added later.

----------------------------------------------------------------------------------------------------------------------------------

5.
preventDefault() vs. stopPropagation() These are two different methods used to control how events behave. • event.preventDefault(): This method stops the default behavior of an event. For example, clicking on a link usually navigates to a new page. Calling preventDefault() on the click event will stop that navigation. Similarly, it can stop a form from submitting or a checkbox from being checked. • event.stopPropagation(): This method stops Event Bubbling. When called, it prevents the event from "bubbling up" to any parent elements. The event will still happen on the element it was triggered on, but it will not be seen by any of its parent listeners.

