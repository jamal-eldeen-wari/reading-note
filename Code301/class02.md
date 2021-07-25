# React: Component Lifecycle Events
Based of the digram the of the react is that the render phase happens first since the order of the digram shows and also the arrows shows that as well.
What makes React special is that it defines as classes or functions.

## There are three phases of the component lifecycle:
First thing in the life cycle is Mounting the updating and then unmounting. 
1. Mounting: Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

2. Updating: These lifecycle events happen during updating in this order.
 static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps.

3. Unmounting: The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

The order of the of the commponent life cycle:
1. Constructor
2. Render 
3. React Update
4. ComponentDidMount
5. ComponentWillUnmount

## What is componentDidMount:
It is a method that is invoked immediately after the component is mounted it is used when we want to load anyrhing using network request or initialize DOM.


# React State vs Props:
Props: are arguments to a function when creating component inside of React to render it we need to pass it to prop.Props is handled outside of the component  
State: Where state is handled inside of the component 
## Big difference:
1. For props you can pass it into component and are handled outside of the component and they are updated also outside. Where state is handled inside of the component and updating inside of the component.
2. Is that when you change the state inside of your application it will rerender that section where as Props you cant actually change them you need to change them outside of the component.

## Where can we use them:
Props are useful when we want to store info inside of the component without hard coding it.
where as the state it is used in counter application or form application.

