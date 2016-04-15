# Getting Started with React and Flux

## What is React?
- React is a open-source user interface framework created by Facebook. It comprises of only the view part of the MVC architecture
- React uses the concept of Virtual DOM
- React encourages us to think in Components
- React uses the FLUX architecture

## React vs Angular
- In Angular when we update / manipulate the DOM, the page gets rerendered and this is an expensive operation.
- Angular maintains a list of watchers in its context. When an event happens on the page, it iterates over the list of watchers inside a digest loop. It runs through a digest cycle and check if something has changed and then accordingly updates the DOM.
- React uses Virtual DOM - a structure internal to React, which mimics the browser DOM. React compares the browser DOM to its own Virtual DOM and figures out the least number of steps necessary to update the Browser DOM to match its Virtual DOM. 
- Since Virtual DOM is not rendered, creating virtual DOMs over and over is faster.
- React runs a diff algorithm to compare the browser DOM to the Virtual DOM
- For any UI update React rerenders its entire Virtual DOM internally without touching the browser and then determining what updates are needed in the Browser DOM based on DOM diffing.
- When we create directives in Angular we attach it to HTML elements and update the DOM, but when we create React components we are not creating HTML elements we create React's Virtual DOM. React's processes are then creating the HTML and updating the DOM

## Thinking in Components
- In order to make the switch to React you need to think in components as everything is a component in React. This encourages reusability and modularity
- When building a UI in react you are composing components together in order to allow react to determine what the DOM should look like and then make updates to the DOM
- Your UI in react is a collection of reusable components. Your UI is an expression of the current state of Data. Each component is concerned with just the data it needs. 

## Setting up React workflow - tools you would need
- babel.js transpiler: it takes your code written in a ECMAScript 2015 and produces code that older browsers can support and run. It also has a built-in JSX transpiler. It can take JSX syntax that React uses and produce the JavaScript code out of it. Babel.js is widely adopted solution for transpiling your code.
- Webpack module bundler:
- Gulp (build system and task runner)
- npm (package manager)
- Bower (package manager)
- Mocha (test framework)
- Jasmine (library for testing)
- ESLint (code linter for ECMAScript 2015)
- Yeoman (scaffolding tool)



