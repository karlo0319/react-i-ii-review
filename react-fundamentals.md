### Remember

Answer these on your own, then compare answers as a group

1.  What is React?
  - React is a JavaScript library that was created and is maintained by Facebook.
  - Focuses on making UI elements and has a virtual DOM
  - A collection of dependencies available in building a React App
  - Uses a component-based architecture and has a unidirectional data flow

2.  What is create-react-app?

   - A tool for putting together a React app in one go
   - Sets up all the toolw we need (for example, initializes a git repo)
   - A development environment with auto-refresh
   - It handles all of the boiler plate setup of React so that we can start building right away.

3.  What is Component Based Architecture?

   - A way to break up a larger project into smaller pieces of code (modular)
   - A way to easily create scalable apps easily
   -Self-sustaining individual blocks of code (components)
   - It makes code highly reusable and easy to debug.

4.  What is JSX?
   - A semantic extension of JS that is like a mix a HTML/JS
   - It is the syntax React uses to describe a user interface
   - Transpiled into JS ultimately

5.  What is the virtual DOM?
   - A memory representation of the DOM that stays in sync with the real DOM
   - A "mock DOM" that keeps a copy of the actual DOM
   - It drastically in some cases increases the performance site (think big site)

   A light-weight copy of the DOM. It makes changes to the user-interface more performant.
  
6.  What is unidirectional (one-way) data flow?
   - Data is passed from parent to children
   - We can get around this by passing info up through events

### Understand

Discuss these questions in pairs if you have a 4-person group

7.  Summarize what happens when you run `create-react-app my-app`
  - A folder is created called 'my-app'
  - The folder includes our boilerplate
  - It creates the git repo for the app AND the package.json necessary to keep track of dependencies

8.  Explain what this code does:

```jsx
import React from "react";

const Mentor = props => (
  <div className="mentor-container">
    <h1 className={props.title === "Lead Mentor" ? "lead" : ""}>Tim Biles</h1>
    <ul>
      <li>Fort Worth, TX</li>
      <li>My email address is timbilestimbiles@gmail.com</li>
    </ul>
  </div>
);

export default Mentor;
```

9.  Explain how data is passed from a parent component to a child component.
  - props

### Apply

Try these on your own, but work together if you start to get stuck.

10.  Use `create-react-app` to create a new React application called `student-directory`

11.  Use the code from `Mentor` above to create a new functional, stateless component called `User` with a list of friends. Hard code the list of friends, do not use state or props.

### Analyze, Evaluate, Create

Discuss these questions as a group

12. What are the benefits and drawbacks of using a tool like create-react-app?
  - Benefits:
      - We can throw together a React app quickly
      - We don't install the individual pieces separately required in a React app
      - Most of the setup 9think config files, etc) is already done for us
  - Drawbacks:
      - It could potentially install something that we don't need leading to a bigger app size. 
      - See link:  https://reactjs.org/docs/create-a-new-react-app.html

13. Compare and contrast JSX with other templating options, such as those used in Angular or Vue

14. Compare and contrast one-way data flow with two-way data binding.
  - One-way = unidirectional
  - Two-way = bi-directional
