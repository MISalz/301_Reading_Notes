# Class05 Reading Notes

React Docs - Thinking in React https://reactjs.org/docs/thinking-in-react.html

<ol><li>What is the single responsibility principle and how does it apply to components? 
a component should ideally only do one thing

</li><li>What does it mean to build a ‘static’ version of your application?
to build a model that never changes but can be reused. like a standard form

</li><li>Once you have a static application, what do you need to add?

</li><li>What are the three questions you can ask to determine if something is state?

<ol><li>Is it passed in from a parent via props? If so, it probably isn’t state.

</li><li>Does it remain unchanged over time? If so, it probably isn’t state.

</li><li>Can you compute it based on any other state or props in your component? If so, it isn’t state.</li>
</ol>

</li><li>How can you identify where state needs to live?
For each piece of state in your application:

Identify every component that renders something based on that state.

Find a common owner component (a single component above all the components that need the state in the hierarchy).

Either the common owner or another component higher up in the hierarchy should own the state.

If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
</li>
</ol>

Higher-Order Functions https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK

<ol>
</li><li>What is a “higher-order function”?
Functions that operate on other functions, either by taking them as arguments or by returning them
</li><li>Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
function within a function return new value = greaterthan > current value (current value)
<img src ="img/2022-03-23_19-46-37 greterthan read05.bmp">
</li><li>Explain how either map or reduce operates, with regards to higher-order functions.
Map will "cleanup" a array to a set type form
Reduce will concat an array into a single value
</li>
</ol><br>
<img src="img/2022-03-23_19-50-18 filtering arrays.bmp"><br>
<img src="img/2022-03-23_19-50-28 map.bmp"><br>
<img src="img/2022-03-23_19-51-01 reduce.bmp"><br>
----
## Things I want to know more about


---
### [Home](https://github.com/MISalz/301_Reading_Notes)