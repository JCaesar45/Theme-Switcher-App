```markdown
# Theme Switcher App

This project is a simple, accessible theme switcher built with HTML, CSS, and JavaScript. It allows users to toggle between different visual themes (e.g., Light and Dark) by clicking a button that reveals a dropdown menu of options. When a theme is selected, the background and text colors change accordingly, and a message is announced via an ARIA live region for accessibility.

---

## Features

- Accessible toggle button with proper ARIA attributes.
- Dropdown menu with theme options, following accessibility best practices.
- Dynamic theme switching by adding/removing CSS classes on `<body>`.
- Live region for announcing theme changes to screen readers.
- Easy to extend with additional themes.

---

## How It Works

- Clicking the **Switch Theme** button toggles a dropdown menu of theme options.
- The dropdown menu appears below the button and can be closed by selecting an option or clicking the button again.
- Selecting a theme:
  - Adds a specific class (`theme-light`, `theme-dark`, etc.) to the `<body>` element.
  - Updates the message in an ARIA live region to notify users of the change.
- The CSS styles are applied based on the theme class to change background and text colors.

---

## Usage

### Setup

1. Copy the HTML, CSS, and JavaScript code provided into your project.
2. Customize the CSS styles within the `<style>` section to define your themes.
3. Add or modify themes in the `themes` array in the JavaScript code:
   ```js
   const themes = [
     { name: 'light', message: 'Light theme activated.' },
     { name: 'dark', message: 'Dark theme activated.' },
     // Add more themes here
   ];
   ``

### How to Interact

- Click **Switch Theme** to reveal theme options.
- Click on a theme (e.g., **Light** or **Dark**) to apply it.
- The background and text colors will change, and a message will be announced for accessibility.

---

## Features & Accessibility

- Button with `aria-haspopup`, `aria-controls`, and `aria-expanded`.
- Dropdown menu with `role="menu"` and `role="menu-item"` for screen readers.
- Hidden attribute controls visibility.
- ARIA live region announces theme changes dynamically.

---

## Customization

- Add more themes by updating the `themes` array and adding corresponding `<li>` items inside the dropdown menu.
- Style each theme in CSS by targeting the class added to `<body>`.
- Adjust the message texts for each theme.

---

## License

This project is open source and free to use.

---

## Support

If you encounter issues or want to extend this project, feel free to fork or contact the maintainer.
```
