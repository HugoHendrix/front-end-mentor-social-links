# Frontend Mentor - Social Links Profile Solution

This is a solution for the [Social Links Profile Challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you enhance your coding skills by building realistic projects.

## Summary

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The Challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page.

### Screenshot

![App Screenshot](https://github.com/HugoHendrix/front-end-mentor-social-links/blob/main/design/solution-frontend-Mentor-social-links-profile.png?raw=true)

## Links

- Solution URL: [FrontEnd Mentor](https://hugohendrix.github.io/front-end-mentor-social-links/)

## My Process

### Built With

- Semantic HTML5 markup
- Custom CSS properties
- Bootstrap
- Mobile-first workflow

### What I Learned

I learned to improve the user experience when interacting with my page, primarily focusing on accessibility and usability. Here are some concepts and practices:

- **Hover and Focus Styling:** Understood the importance of styles for `:hover` and `:focus` to provide visual feedback to users during interaction.

- **Accessibility:** Learned how adding specific styles for focus (`:focus`) aids users navigating by keyboard or using screen readers, providing a more inclusive experience.

- **Responsive Styling:** Delved into responsive styling principles to ensure a good user experience on different devices, especially focusing on mobile improvement.

- **Element Selection:** Discovered the `:focus-within` selector, allowing the application of styles when any child element of a container is focused. Useful for highlighting an entire container when any part of it is interactive.

- **Removing Default Styles:** Learned to remove default browser styles, such as the border when focusing on links, providing a more customized and consistent appearance.

These practices are essential for creating engaging, functional, and accessible web interfaces.

```css
/* Adds styling for focus on links */
ul li a:focus {
  outline: none; /* Removes default browser border */
  box-shadow: 0 0 0 3px var(--Blue-Hendrix); /* Adds a border around the link when focused */
}

/* Enhances focus experience on mobile devices */
ul li a:focus:not(:hover) {
  color: var(--Off-Black);
  background-color: var(--Blue-Hendrix);
}

/* Adds styling for focus on list items */
ul li:focus-within {
  background-color: var(--Blue-Hendrix);
  color: var(--Gray);
}

/* Adds styling for focus on list items and their links */
ul li:focus-within a {
  color: var(--Gray);
}

/* Removes default Bootstrap button border when focused */
.btn:focus {
  outline: none;
  box-shadow: none;
}
```

## Continued Development

- Learn more about Bootstrap classes.
- Deepen understanding of:
  - Code reuse and refactoring.
  - Responsiveness.
  - BEM (Block Element Modifier).
  - Accessibility.

### Useful Resources

- [Bootstrap Cheat Sheet](https://bootstrap-cheatsheet.themeselection.com/) - A quick reference sheet for Bootstrap classes. Useful for exploring and understanding the possibilities offered by the framework.
- [Maujor](https://www.maujor.com/) - The website of Mr. Maurício Samy Silva, providing valuable resources and knowledge about web development.

## Author

- Frontend Mentor - [@HugoHendrix](https://www.frontendmentor.io/profile/HugoHendrix)
- Linkedin - [Hugo Hendrix](https://www.linkedin.com/in/hugohendrix/)

---

[![Leia em Português](https://img.shields.io/badge/Read%20in-Portuguese-green)](README.md)
