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

## Footer Structure:
The Footer component follows a simple structure:

- Footer: Parent component responsible for rendering the footer section.
- Navigation Links: Provides links to various sections of the application such as Home, Blog, Save/Bookmark, Profile/User. etc.
- Blog Button: Represents a specific action within the app, allowing users to access Blog post section.

## React Icon Implimentation:
The Footer component utilizes the react-icons library to import and display icons for navigation links and interaction elements. 
Icons are imported as components and integrated within the Footer component for seamless rendering.

### To import react icons into the Footer component:

```
import React from 'react';
import { FaHome, FaSearch, FaBookmark, FaUser } from 'react-icons/fa'; // Importing required icons from react-icons/fa
```

### Flow diagram of component relationship:
![flowdiagram!](images/flow-daigram.jpg)

### Diagram:
1. The App represents the overall structure of the application.
2. The Header, Main Content and footer components representing other sections of the application.
3. The Main Section contains the primary content of the application.
The Footer component is located at the bottom of the application layout. Each component is interconnected, with the Footer being
a part of the overall layout and providing navigation links and interaction to the user.


## Code Snippet for our footer components:
```
    import React from 'react';
    import { Link } from 'react-router-dom'; // Importing Link component from React Router for navigation
    import { FaHome, FaSearch, FaBookmark, FaUser } from 'react-icons/fa'; // Importing required icons from react-icons/fa
    
    function Footer() = {
      return (
        <footer>
          <nav>
            <ul>
              <li>
                <Link to="/">
                  <FaHome /> Home
                </Link>
              </li>
              <li>
                <Link to="/search">
                  <FaSearch /> Search
                </Link>
              </li>
              <li>
                <Link to="/bookmark">
                  <FaBookmark /> Save/Bookmark
                </Link>
              </li>
              <li>
                <Link to="/profile">
                  <FaUser /> Profile
                </Link>
              </li>
            </ul>
          </nav>
        </footer>
      );
    };
    
    export default Footer;
```
