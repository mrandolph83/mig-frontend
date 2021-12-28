# Movie Idea Gen Devlog
## Objectives
- Update Javascript Movie Idea Gen Project into Component-based React application with Redux State management
- Implement TDD fundamentals using Jest
- Approach SPA as a single window updating to new Components, rather than one long contoinuous window
- Demonstrate single responsibility principle with each Component

## Component Sructure/Function
### APP (App.js)
- Wrap all Redux functionality into App.js
- Contains HEADER.JS and FOOTER.JS

### WELCOME (WelcomeContainer.js)
- Container for Movie theater background element, which holds Login.js, Signup.Js, and BeginGen.js
- BeginGen.js allows user to select to generate a new idea (leading to PitchGen.js), or update a previous idea (PitchList.js)

### PITCH 
- Navbar.Js is contained under this
- IdeaList.js allows user selection of ideas they have 
-


