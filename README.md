What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

getElementById: Returns the element with the specified id. Since IDs should be unique, it always returns a single element.

getElementsByClassName: Returns a live HTMLCollection of all elements with the specified class name. The collection updates automatically if the DOM changes.

querySelector: Returns the first element that matches a given CSS selector (e.g., #id, .class, div > p).

querySelectorAll: Returns a static NodeList of all elements matching the CSS selector. Unlike getElementsByClassName, this list does not update automatically.

How do you create and insert a new element into the DOM?

To create a new element in dom i use document.createElement() method.
To insert it i use document.appendChild() method.

What is Event Bubbling and how does it work?

Event bubbling is the JavaScript mechanism where an event, after being triggered on a specific DOM element, propagates or "bubbles up" through its ancestor elements (parents, grandparents, etc.) all the way to the document's root

What is Event Delegation in JavaScript? Why is it useful?

A technique where instead of attaching event listeners to multiple child elements, a single listener is attached to a parent element.

The event’s target (event.target) is used to determine which child triggered it.

It used to improves performance, reduces memory usage and works for dynamically added elements.

What is the difference between preventDefault() and stopPropagation() methods?

preventDefault(): Prevents the default browser behavior for an event (e.g., stops form submission, blocks link navigation).

stopPropagation(): Prevents the event from bubbling up (or capturing down) the DOM tree, stopping parent elements from receiving the event.
