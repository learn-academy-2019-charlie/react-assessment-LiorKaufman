# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs)
- React is a modern, efficient answer to complex UI applications
- React is a flexible library that plays the role of V in an MVC framework

 
 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.
 
 
 //Your Answer
 
 smart components have state inside of them and so they can have their own individual logic that affects only them 
 Dumb components do not have state thus they only render to the screeen 
 
 //Googled Answer
 
 Smart components (or container components) on the other hand have a different responsibility. Because they have the burden of being smart, they are the ones that keep track of state and care about how the app works.
 Dumb components are also called ‘presentational’ components because their only responsibility is to present something to the DOM. Once that is done, the component is done with it. No keeping tabs on it, no checking in once in a while to see how things are going. Nope. Put the info on the page and move on.
 
#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?
 
 
 //Your Answer
 
 yarn add adds a new package or tells yarn to download something the modules should be update 
 //Googled Answer
 
 This means running yarn add [package-name] to install it into your project. This will also update your package.json and your yarn.lock so that other developers working on the project will get the same dependencies as you when they run yarn or yarn install .
#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

1.added extends
2. made an array for recipes
3. move let recipes to happen in the render method but before return 
    import React, { Component } from 'react';
    
    class Recipes extends Component {
      constructor(props){
        super(props)
        this.state = {
          recipes:[ 
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}]
      
        }
      }

      render() {
        let recipes = this.state.recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })
        return (
    
          
    
          <ul>
            {recipes}
          </ul>
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)
 
 //Your Answer
 password
 number
 email
 submit
 
 //Googled Answer
 
 
 #### 7. How would you explain state to a friend who doesn't know code?
 
 //Your Answer
 It is a way for a part of the program to keep track of its own data 
 
 //Googled Answer
 What is state? The heart of every React component is its “state”, an object that determines how that component renders & behaves. In other words, “state” is what allows you to create components that are dynamic and interactive.
 
 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.
 
 
 //Your Answer
 
 state are local for each component and need to be declared inside the componenet, props are data that it is passed down from parent componene tto child componenet
 unlike state a component cannot change its props
 
 //Googled Answer
 
   What's the difference between state and props in React? In a React component, props are variables passed to it by its parent component. ... Props should never be changed in a child component, so if there's something going on that alters some variable, that variable should belong to the component state.Nov 8, 2018
#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.

I feel that with react I need to have a different mindset to the language than just plain JS or other programming languages. I found the acces to the DOM to be harder with react and only after some more time working with react I realized I should not have to work so much with the DOM.
By changing my mindset to work more with componenets, props and states my ability to write react code improved. 
I feel also writing a program from scratch really makes you learn the best as it requires you to reallu understand what you are tyign to build. 
