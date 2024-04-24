# Eco-Agric-Frontend-Doc
### Introduction
The Frontend team will implement the UI design using the React javaScrip Library.

# Header Component
The Header component is designed to be a reusable component that display the brand logo, the notification icon, Add category buttons that will use axios
to map all the post component by category through API endpoint.

# Post Component

# Footer Component
The Footer component work's as navigation with React icons to enhance visual appeal and clickable functionality, improving user experience.

## Introduction
The Footer component is designed to be a reusable component that provides essential navigation links and interaction options to users at 
the bottom of the application. It utilizes React Router for navigation between different sections of the app and integrates Font Awesome icons for visual representation.

For our icons and link (navigation link for the footer), we need to install two dependencies, After installation then we import then into our component

**Two dependencies to install:**
- npm install react-router-dom
- npm install react-icons

**Two dependencies that we import:**
- import React from 'react';
- import Footer from './Footer';

## Importing the Footer component into Our project:
- import Footer from './Footer'; into the App.jsx Component.
- Place the Footer component at the bottom of your application layout.

Once installed and imported, we can use the Footer component within your React application by simply rendering it as part of your layout.
The component automatically provides navigation links and interaction elements at the bottom of the application.

## Code snippet:
```
    import React from "react";
    import Footer from "./Footer";
   
    const App = () => {
      return (
        <div className="app">
          {/* Other application content */}
          <Footer />
        </div>
      );
    };
    
    export default App;
```
