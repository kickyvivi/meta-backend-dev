# Notes for Week 3

## Introduction to UI Frameworks and Libraries

### Responsive Design:
- Flexible Grid
- Fluid images
- Media queries
- They all together form the responsive design
- Breakpoint : FIXED, FLUID, HYBRID Grid

### Bootstrap:
- Bootstrap is a library of CSS and JavaScript code that you can combine to quickly build visually appealing websites.
- Bootstrap comes with multiple components for very fast construction of multiple components, or parts of components.
- Bootstrap comes with a pre-made set of CSS rules for building a responsive grid.

### Getting started with Bootstarp:
- `<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">`
- `<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"-</script>`
- **`container - row - col`**

### Using bootstrap styles:
- infixes and modifiers
- breakpoint is the trigger for changing layout
- You will use an infix to indicate the breakpoint in Bootstrap CSS rules.
- Modifers :
    - Primary
    - Secondary
    - Success
    - Info
    - Warning
    - Danger
    - Light
    - Dark
    - Alerts :
- Primary - Displays the alert in Blue (Default bootstrap color)
- Danger - Displays the alert in Red

### Bootstrap grid:
- 12 columns available : fluid or fixed
- container is the root element
- width is determined based on current responsive breakpoint

### Bootstrap components:
- Pre made set of UI elements and styles
- E.g.: Alert messages, navigation menu 
- We are using the card and alert components in the `bootstrap-components.html`
    - card
    - card-img-top
    - card-title
    - card-text
    - alert alert-info
    - role="alert"
    - badge bg-primary

### Using Bootstrap documentation:
- [Documentation](https://getbootstrap.com/docs)
- Sample added at the end of [bootstrap-components.html](./Intro%20to%20UI%20Frameworks%20and%20Libraries/bootstrap-components.html)

### Other CSS frameworks and libraries
- Foundation - [Official website](https://get.foundation/)
    - Similar to bootstrap
    - One prominent feature of Foundation is that it can be used to style content for sending via email.
- Pure.css - [Official website](https://purecss.io/)
    -  It is designed to be minimal in file size
    - Less loading time
- Tailwind CSS - [Official website](https://tailwindcss.com/)
    - Utility based approach
    - This means that the framework provides many CSS classes with a single purpose
- UIKit - [Official website](https://getuikit.com/)
    - UIKit is a lightweight CSS framework featuring a small set of responsive components. Its simple design allows developers to easily customize the style rules and visuals.
- MVP.css - [Official website](https://andybrewer.github.io/mvp/)
    - MVP.css is a small CSS library that automatically styles HTML elements without needing to apply CSS classes to them. 
    - Minimal Viable Product, a product with sufficient features to demo to customers or other business stakeholders.

## Introduction to React

### Static and dynamic content
- Web server loads the page
- Application server loads the dynamic content (Backend)
- Caching
    - A saved copy of dynamic content kept in web server.
    - If content is requested again, web server does not have to send request again to application server
    - Web server keeps updating the cache with latest version with time or subsequent requests

### Single page applications
- Traditional applications
    - Multt page websites
    - Resource intensive
    - Slow site browsing experience
- Solution
    - SPA
    - One HTML page is send from server to browser and it keeps updating with user interation
    - Faster interaction
    - Rewrites current webpage with user interaction instead of loading new pages
    - Bundling:
        - Load all HTML, CSS and JS in one go when browser requests the application
    - Lazy loading:
        - When browser requests, the web server returns the min. HTML, CSS and JS needed to load the application
        - Additional resources are loaded as needed
    - Data is sent from Web server to browser as JSONs instead of loading a new website for each dynamic request
    - JSON contains only the required data and SPA updates the HTML according to the data
    - The web browser updates the webpage by inserting the ***template*** with items replaced by items in JSON object
    - Website with more than 1 pgae:
        - Different pagesd are broken down into templates/views
        - HTML is updated using the JSON returned by web server

### What is Reacts?
- Front end develeopment
- Working with components
- Open source library
- SPA and mobile applications with React native
- React component: Small piece of user interface
    - E.g.: Music player component, photo gallery component, maps component, video player component
- Isolated development and testing
- Reuse components across multiple sections
- E.g.: **User icon component** for profile picture - Reused in different parts of the website
- Features:
    - Write less code to implement functionality in a web browser.
    - Maintain code in the long term.
    - Re-use components.
    - Simplify testing.

### How React works?
- React creates and updates a virtual DOM (Document Object Model) to make webpages faster
- **Reconciliation**:  With each change to components the new virtual DOM is compared to the previous virtual DOM and only the changes are updated in the browser DOM instead of recomputing the browser DOM again
- This way browser will update only certain HTML elements instead of recreating the entire page

### Virtual DOM and Fiber Architecture 
- The Fiber Architecture allows React to incrementally render the web page
- The highest priority changes, the elements visible to the user, are updated first. While lower priority changes, the elements not currently displayed, are updated later
- A long web page > User scrolled to the bottom and updated something > Some text need to be updated at the bottom and also at the top > The bottom text is first updated on priority as the top portion is not visible on the browser currently and that takes low priority.

### Other libraries
- Lodash - [Official Website](https://lodash.com/)
    - Lodash provides common logic such as these as a utility library to save you time as a developer.
- Luxon - [Official Website](https://moment.github.io/luxon/#/)
    - Luxon helps you work with dates and times by providing functions to manipulate and display them.
- Redux - [Official Website](https://redux.js.org/)
    - When building a web application, you'll need to keep track of its state
    - Think of when you shop online. The web application tracks items currently in your shopping cart. When you remove an item from the cart, the application needs to update what displays on the screen.
- Axios - [Official Website](https://axios-http.com/)
    - Fir working with APIs
    - The Axios library helps to simplify sending HTTP requests and processing the response. 
    - It also provides advanced features allowing you to cancel requests and to change data received from the web server before your application uses the data.
- Jest - [Official Website](https://jestjs.io/)
    - Automated test and reporting
