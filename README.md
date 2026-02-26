1.  **What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?**  
   `getElementById` returns a single element because IDs must be unique within a document.  
   `getElementsByClassName` returns a live HTMLCollection of all elements that share the specified class name.  
   `querySelector` returns the first element that matches a given CSS selector, requiring the use of `.` for classes or `#` for IDs.  
   `querySelectorAll` returns a static NodeList containing every element that matches the CSS selector.

2.  **How do you create and insert a new element into the DOM?**  
   Use `document.createElement()` to generate a new element. After creating it, you can set its content or attributes via properties like `textContent` or `innerHTML`. Finally, insert the element into the DOM by calling `appendChild()` or `insertBefore()` on a parent node.

3.  **What is Event Bubbling? And how does it work?**  
   Event bubbling is the propagation of an event from the target element upward through its ancestors. The event triggers first on the deepest element, then bubbles up to its parent, then to its grandparent, continuing until it reaches the document root.

4.  **What is Event Delegation in JavaScript? Why is it useful?**  
   Event delegation is a technique where a single event listener is attached to a parent element to handle events for all child elements, leveraging event bubbling. This approach is beneficial because it reduces memory usage by minimizing the number of listeners, works for dynamically added elements, and leads to cleaner, more maintainable code.

5.  **What is the difference between preventDefault() and stopPropagation() methods?**  
   `preventDefault()` cancels the browser's default behavior for an event (e.g., stopping a form submission or link navigation).  
   `stopPropagation()` halts the event from bubbling further up the DOM tree, preventing parent elements from receiving the event.