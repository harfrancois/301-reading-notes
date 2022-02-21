What is the single responsibility principle?

single responsibility principle - a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents. how does it apply to components? It helps you figure out what should or should not be its own component. 

What does it mean to build a ‘static’ version of your application?

Setting up the bare bones of your UI with out any features.

Once you have a static application, what do you need to add?

Build components that reuse other components and pass data using props

What are the three questions you can ask to determine if something is state?

- Is it passed in from a parent via props?

-Does it remain unchanged over time?

-Can you compute it based on any other state or props in your component?

How can you identify where state needs to live?  

You have to determine the hierarchy of your components. Figure out what depends what to function 

What is a “higher-order function”?

Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

It will return M if M is greater than N.

Explain how either map or reduce operates, with regards to higher-order functions.

Map and reduce depends on another function to return a new array.