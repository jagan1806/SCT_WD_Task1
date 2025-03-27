# Task 01: Responsive Landing Page
## Project Overview
A modern, fully responsive landing page with an interactive navigation menu that changes color/style when scrolled or when hovering over menu items. The navigation menu maintains a fixed position and remains visible on all pages.
## Features

- **Interactive Navigation Menu**
  - Color/style changes on scroll
  - Visual feedback on hover
  - Automatic highlighting of current section
  - Fixed position for constant accessibility

- **Responsive Design**
  - Mobile-first approach
  - Adapts to all device sizes (mobile, tablet, desktop)
  - Hamburger menu for smaller screens

- **Modern UI Elements**
  - Clean, professional design
  - Smooth scrolling navigation
  - Subtle animations and transitions
  - Consistent color scheme and typography

- **Page Sections**
  - Hero/Welcome section
  - About section
  - Services section
  - Portfolio section
  - Contact form
  - Footer with social links

## Technologies Used

- HTML5 for structure
- CSS3 for styling (custom properties, flexbox, grid)
- Vanilla JavaScript for interactivity
- No external frameworks or libraries

## Implementation Details

### Navigation Features

The navigation has been implemented with several interactive elements:

```javascript
// Change navbar style on scroll
window.addEventListener('scroll', () => {
    const navbar = document.querySelector('.navbar');
    if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
    } else {
        navbar.classList.remove('scrolled');
    }
});

// Highlight active menu item based on scroll position
window.addEventListener('scroll', () => {
    const sections = document.querySelectorAll('section');
    const navLinks = document.querySelectorAll('.nav-links li');
    
    // Logic to determine current section and highlight nav item
});
```

### Responsive Approach

Media queries are used to ensure the layout works across all device sizes:

```css
/* Responsive styles */
@media screen and (max-width: 768px) {
    .menu-toggle {
        display: block;
    }

    .nav-links {
        position: fixed;
        top: 80px;
        left: -100%;
        width: 100%;
        height: calc(100vh - 80px);
        background-color: #1a1a2e;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transition: all 0.5s ease;
    }

    /* Additional responsive styling */
}
```

## How to Use

1. Clone this repository
2. Open `index.html` in your web browser
3. Navigate through the sections using the menu
4. Explore the responsive behavior by resizing your browser

## Future Enhancements

- Add dark/light theme toggle
- Implement form validation and submission
- Create additional pages for services and portfolio items
- Add animation libraries for enhanced visual effects

## Screenshots

[Insert screenshots here]

## License

This project is part of the SkillCraft Technology internship program.
