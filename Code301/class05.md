# Thinking in React:
## How would you break a mock into a component heirarchy?
Since you’re often displaying a JSON data model to a user, you’ll find that if your model was built correctly, your UI (and therefore your component structure) will map nicely. That’s because UI and data models tend to adhere to the same information architecture. Separate your UI into components, where each component matches one piece of your data model.

## What is the single responsibility principle and how does it apply to components?
it is used if we decided to create a new function or object. that is, a component should ideally only do one thing.

## What does it mean to build a ‘static’ version of your application?
To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

## Once you have a static application, what do you need to add?
you will need to install a special preset for Flow.

## What are the three questions you can ask to determine if something is state?
1. Is it passed in from a parent via props?
2. Does it remain unchanged over time?
3. Can you compute it based on any other state or props in your component? 

## How can you identify where state needs to live?
Below there is some ways to know to be live:
1. Identify every component that renders something based on that state.
2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
3. Either the common owner or another component higher up in the hierarchy should own the state.
4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
