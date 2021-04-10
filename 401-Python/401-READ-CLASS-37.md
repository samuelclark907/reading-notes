## REACT

- React is a JS library
- The smallest React example looks like this:

ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

### JSX

`const element = <h1>Hello, world!</h1>;`

- This funny tag syntax is neither a string nor HTML.

- It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

- React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

[Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)

### Rendering Elements

An element describes what you want to see on the screen:

`const element = <h1>Hello, world</h1>;`

- Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

[Rendering Elements](https://reactjs.org/docs/rendering-elements.html)

### Components and Props

- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components.

[Components and Props](https://reactjs.org/docs/components-and-props.html)

### State and Lifecycle

[State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

### Handling Events

[Handling Events](https://reactjs.org/docs/handling-events.html)

