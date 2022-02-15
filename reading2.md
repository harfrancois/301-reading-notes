# React: Component Lifecycle Events

source https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093

React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. Mounting, Updating, and Unmounting are the three phases of the component lifecycle.

## Mounting
The instance something is created

mounting phase - Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount

## Updating
Anytime a component is updated or state changes.

static getDerivedStateFromProps
shouldComponentUpdate
render
getSnapshotBeforeUpdate componentDidUpdate UNSAFE_componentWillUpdate UNSAFE_componentWillReceiveProps

## Unmounting
final phase of the lifecycle when a component is being removed.

## constructor()

constructors can be used to assign state using this.state or to bind event handle methods to an instance.

## static getDerivedStateFromProps()

This method exists for rare cases where the state relies on changes in props over time.

## render()

Render is the only required method in a class component.

## componentDidMount()

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM.

## shouldComponentUpdate()

The default behavior in react is to rerender after every state change.

If shouldComponentUpdate() returns false, then UNSAFE_componentWillUpdate(), render(), and componentDidUpdate() will not be invoked.

## getSnapshotBeforeUpdate()

Allows you to capture a picture of the DOM to check it before actually changing anything.

## componentDidUpdate()
This method is useful for performing network requests after a change has occurred.

## componentWillUnmount()
This method allows you to clean up the DOM and netwrok requests/ subscriptions.

## React State Vs Props

What types of things can you pass in the props?  

- information you want to display.


### What is the big difference between props and state?

- props you pass in to a component
state you handel in side that component props are handel outside a component.

### When do we re-render our application? 

- when the props change.

### What are some examples of things that we could store in state?

- data that re-render and update based on somthing the user has done.