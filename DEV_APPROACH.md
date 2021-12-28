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
- API Get request calls for MyIdeas (Current User Ideas)
- BeginGen.js allows user to select to generate a new idea (leading to PitchGen.js), or update a previous idea (PitchList.js)

### PITCH 
- API get request updates state of 
- Navbar.Js is contained under this
- IdeaList.js allows user selection of ideas they have (state of MyIdeas) 
- PitchGen.js generates pitch for user, allowing them to mix/match genres and shuffle between any individual element
- PitchGen.js contains GenreBoxes.js, which is the tool that 
allows user to select Genres to include or uninclude in plot generation
- PitchCustom.js allows users to finalize their initial pitch. Updates with pre-filled current state of "character, setup, pitch" if user went through Pitch Generator First
- PitchCustom is the entry point to the Brainstorm phase

### BRAINSTORM
- Brainstorm{step#}.js steps through each part of the Brainstorm process, each one having BrainstormSteps.js and Timer.js
- BrainstormSteps.js gives users ability to navigate between each of the brainstorm steps. Background changes color each time data is submitted (stretch) 
- Timer.js is a simple 15:00 timer that user can choose to use at each step
- BrainstormReview.js simply is a display of current state of all Brainstorm{step#} data. Allows you to submit (Create in API) your idea, or Save as PDF (React Library Function?)

### RESOURCES
- Resource.js shows resources utilized in the creation of the app



