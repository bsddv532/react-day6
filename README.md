# React-day6 Practice

---
## Q.1 What is Virtual DOM ?

 DOM stands for Document Object Model. Whenever any HTML, CSS, javascript application gets loaded for the first time on the browser then the browser creates Document object model of that file, and whenever we changes anything in application then the complete DOM is rerendered again and again. 
   
   But in case of react, the DOM is created whenever our react components mounted on the screen for the first time. Now when we makes any changes on the screen like button click because of which the state variable gets updated so in this case the real DOM not directly changed the updates, for this in react we have a concept known as Virtual DOM. In react we use virtual DOM to update the real DOM. 
   
   In react we are having two virtual doms, one virtual dom gets created at the time of mounting of react component so it is a copy of our real DOM, and another virtual DOM contains all the new changes, updated values of state variables. Now both the virtual DOMs get compared with each other and will check for the new changes, this complete procedure is known as Diffing algorithm. Now the new changes will be updated in our Real DOM, this procedure is known as Recoinciliation.
   
 ---
 
 ## Q.2 What is SPA ?
 
  SPA stands for Single Page Application. It means whenever any event is occured in an application then that application not getting reloading , such type of appliactions is known as Single Page Application. When we create React application using CRA, it always create the application which will be Single page application.
  In react by using router we create single page applications.
  
   #### For example 
   When we click on the button or select any option in navigation bar then our website is not getting reloading in browser it directly updates the content of our website such type of websites are the example of SPA.
  
---

## Q.3 Phases and Methods of life cycle of a component

There are three phases of life cycle of a component :-
1. Mounting
2. Updating
3. Unmounting

### 1. Mounting Phase :-
   When an instance of component is created and inserted into DOM.
   #### i. constructor()
   #### ii. static getDerivedStateFromProps()
   #### iii. render()
   #### iv. componentDidMount()
   
### 2. Updating Phase :- 
   When a component is being re-rendered based on change in state or props.
   #### i. render()
   #### ii. componentDidUpdate()
   

### 3. Unmounting Phase :-
   When a component is being removed from the DOM. 
   #### i. componentWillUnmount()
   
---

## Q.4 Difference between Class Component and Functional Component

 #### Class Component :- 
   1. A class component requires you to extend from React. Component and create a render function which returns a React element.
   2. Class component can be used when you are doing data operations and server calls.
   3. It is also known as Stateful components because they implement logic and state.
   4. It must have the render() method returning JSX.
   5. It contains lifecycle methods.
   6. Constructor are used as it needs to store state.

   
 #### Function Component :-
   1. A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element.
   2. Functional components can be used mostly when we need to create dumb or stateless components.
   3. It is also known as Stateless components as they simply accept data and display them in some form, that they are mainly responsible for rendering UI.
   4. It does not have state variables, it uses hooks like useState, useParams, etc.
   5. It uses hooks like useEffect in place of react life cycle method.
   6. Complete constructor structure is not required in these components, so they are easy to handle.

---

## Q.5 In react why we move from class component to function component ?
As we know javascript is a functional programming language, thats why we are moving from class component to function components.

---
## Q.6 What is routing ?
Routing is a process in which a user is directed to different pages based on their action or request. ReactJS Router is mainly used for developing Single Page Web Applications. React Router is used to define multiple routes in the application.

When a user types a specific URL into the browser, and if this URL path matches any 'route' inside the router file, the user will be redirected to that particular route.
