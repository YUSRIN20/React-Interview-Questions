 # React Interview Questions

## 1. What is the **role of react** in software development? **V.IMP**

## 2. What is React?
 - React is an open source Javascript Library.
 - React is used for building userInterfaces(UI)
 - We need react because react simplifies the creation of **SPA** by using resuable components.

## 3. What is **SPA(Single Page Application)**
 - A Single Page Application (SPA) is a web application that have only one **single web page**.
 - Whenever user do some action on the Website, then in response content is dynamically updated without refreshing or loading a new page.

## 4. What are the advantages of React? **V.IMP**
 - Simple to build Single Page Application (by using Components)
 - React is cross platform an open source(Free to use)
 - lightweight and very fast(virtual DOM)

## 5. What are **disadvantages** of React?
 -  React is not a good choice for very small applications.

## 6. What is the difference between **React** and **Angular**?

## 7. What is DOM?
 -  The DOM (Document Object Model) represents the web page as a **Tree-like structure** which alloes javascript to dynamically acess and manipulate the content and structre of a web page.

## 8. What is the difference between **DOM** & **Virtual DOM**?**V.IMP**
  - React uses a Virtual DOM to effectively update the UI without re-render the entire page, which helps improve performance and make the apllication more responsive.

## 9.What are React Components?
 - In react, a component is a **resuable building block** for creating user interfaces.

 ## Chapter-2 Main Files & Folders

## 10.What is npm? What is the role of node_modules folder?
 - NPM is used to **manage** the dependancies for your react Project,including the React library itself.
 - **Node Modules:** node_modules folder contains all the dependancies of the project, including the React libraries.

## 11.What is role of **Public** folder in React?
 - Public folder contains **static assets** that are served directly to the user's browser, such as images, fonts, and the index.html file

## 12. What is the role of **src** folder in React?
 - In React, src folder is used to store all the source code of the application.

## 13. What is the role of **index.html** page in react? **V.IMP**
 - Index.html file in a React project is the entry point to the application.

## 14. What is the role of **App.js** file in React? **V.IMP**
 - App.jsx is the top/main/root level component in a React application, and it is responsible for rendering all of the other child components

## 15. What is the role of **function** & **return** inside App.jsx?
 - In React, a function is a JavaScript function that returns a react element.

## 16. Can we have a function without **return** inside App.js?
  - Yes
```javascript
import './App.css'

function App(){
    console.log('clicked!')
}

export default App
```

## 17. What is the role of **export default** inside App.jsx?
 - It is used to make this App Component available for **import** using 'import'statement in other files.

## 18. What is the role of **index.js** file, **ReactDOM** and **render** method in react?
 - **ReactDOM** :ReactDom is a javascript library which convert your components (Which are Written in React Syntax) to the actual browser DOM.
 - **Index.js** :Index.js file is the javascript file which renders all the components and replace the root element of index.html file with the newly rendered root element

## How React App **load** and display the components in browser?
 -   

## Chapter-3-JSX

## 20. What is JSX?
 - JSX means (Javascript XMl) is a extension for javascript library recommended for react for what UI should Look like and its combine HTML & Javascript like syntax to create react elements

## 21. What are the advantages of JSX? **V.IMP**  
 - Advantage of JSX
     * Improve code readability and writability.
     * Error checking in advance (Type safety).
     * Support Javascript expressions.
     * Improved performance
     * Code reusability
## 22. Can browser read a JSX file> What is **Babel**?
 - No, Browser will not understand the JSX code directly, after converting the JSX  react code to javascript by using babel library then browser will understand the javascript code.
 - **Babel:** Babel in React is used to transpile JSX syntax into regular javascript which browser can understand.

## 23. What is Transpiler?
 - A transpiler is a tool converts source code from one programming language to another.
## 24. Is it's possible to use JSX without React?
 - it's possible to use JSX without React by creating your transpiler like Babel.
 - However, this is not recommended since JSX is tightly integrated with React and relies on many React-specific features.

## 25. What is the role of **fragment** in React? 
 - In React, a fragment is a way to group a list of children without adding extra nodes to the **DOM**

## 26. How do you iterate over a **list** in JSX? What is **map()** method? **V.IMP**
  - map() method allows you to iterate over an array and modify its elements using a callback function.
```javascript
function App(){
    // Define an array of numbers
    const numbers = [1,2,3,4,5]

    return(
        <>
        {
            numbers.map((item)=>(number*2))
        }
        </>
    );
    // output:2 4 6 8 10
}
```
## What are **props** in JSX?
 - Props are properties passed to a component from its parent and they are immutable
```javascript
function app(){
    return (
        <>
         <ChildComponent name="Happy" purpose="Interview">
        </>
    )
}

function ChildComponent(props){
    return <div>{props.name},{props.purpose}!</div>
}
// Output:Happy,Interview!
```
## What are **spread operator?**
 - The spread operator {...} is used to expand or spread an array or object.
```javascript
function app(){
    return (
        <>
          <ChildComponent name="Happy" purpose="Interview">
        </>
    )
}

function app(){
    const props = {name:"Happy",purpose:"Interview"};

    return (
        <>
          <ChildComponent {...props}/>
        </>
    )
};

function ChildComponent(props){
    return <div>{props.name},{props.purpose}!</div>
}
// Output:Happy,Interview!
```

## 29. What are the types of conditional **rendering** in JSX?
 - Conditonal Rendering 
     * if/else statements
     * Ternary Operator
     * && Operator
     * Switch statement

## 30. 
