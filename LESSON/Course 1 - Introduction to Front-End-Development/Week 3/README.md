# Notes for Week 3

## Responsive Design:
- Flexible Grid
- Fluid images
- Media queries
- They all together form the responsive design
- Breakpoint : FIXED, FLUID, HYBRID Grid

## Bootstrap:
- Bootstrap is a library of CSS and JavaScript code that you can combine to quickly build visually appealing websites.
- Bootstrap comes with multiple components for very fast construction of multiple components, or parts of components.
- Bootstrap comes with a pre-made set of CSS rules for building a responsive grid.

## Getting started with Bootstarp:
- `<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">`
- `<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"-</script>`
- **`container - row - col`**

## Using bootstrap styles:
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

## Bootstrap grid:
- 12 columns available : fluid or fixed
- container is the root element
- width is determined based on current responsive breakpoint

## Bootstrap components:
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

## Using Bootstrap documentation:
- [Documentation](https://getbootstrap.com/docs)
- Sample added at the end of [bootstrap-components.html](./Intro%20to%20UI%20Frameworks%20and%20Libraries/bootstrap-components.html)

## Other CSS frameworks and libraries
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