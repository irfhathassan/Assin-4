 ## 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
 Ans:we use getElementById() to select one element using its id.
 We use getElementbyClassName() to select many elements using classname.
 We use querySelector() to select the first matching element by using CSS selector.
 We use querySelectorAll() to select all matching elements by using CSS selector.
## 2. How do you create and insert a new element into the DOM?
 Ans:At first, we create an element like:const div = document.createElement("div");
     then we add text to it.exp:div.innerText = "Hello";
    once these are done,we then have to add it to the page
    exp:document.body.appendChild(div);
    thats how we create and insert a new element into the DOM.
## 3. What is Event Bubbling? And how does it work?
   Ans:Event bubbling means when you click something,the event moves from the child element to the parent element.
      for example: if we click a button inside a div first,the button's click runs.then the div's click event runs.and then the body's click event runs
    So,the event goes from child to parent.This upward movementis called event bubbling
 ## 4. What is Event Delegation in JavaScript? Why is it useful? 
     Ans:Event delegation means adding one event listener to a parent instead of many child elements.It works because of event bubbling.
       It is very usefull because it needs less code,it performs better and it works for new elements added later.
 ## 5. What is the difference between preventDefault() and stopPropagation() methods?
    Ans: The difference between preventDefault() and stopPropagation() is that:
    preventDefault() stops the browser's normal action and stopPropagation() stops the event from goingto parent elements
    So, we can say, preventDefault() stops browser action and stopPropagation() stops event moving up
