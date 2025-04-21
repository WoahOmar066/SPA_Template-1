# Dashboard Template

A clean, responsive dashboard template with dark/light theme support, sidebar navigation, and content switching functionality.

![Dashboard Preview](preview.png)

## Features

- **Responsive Design**: Adapts to different screen sizes
- **Dark/Light Theme**: Toggle between light and dark modes with automatic preference saving
- **Interactive Sidebar**: Easily navigable sidebar with icon support
- **Dynamic Content Switching**: Content sections change based on navigation selection
- **Minimal Dependencies**: Lightweight with no external JavaScript libraries required
- **Custom CSS Variables**: Easy theming and customization
- **Modern UI Elements**: Clean, contemporary design language

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic knowledge of HTML, CSS, and JavaScript

### Installation

1. Download or clone the repository
2. Open `template1.html` in your browser to see the dashboard

## Usage

The dashboard template is contained in a single HTML file with inline CSS and JavaScript for simplicity. To use it in your project:

1. Copy the `template1.html` file to your project directory
2. Modify the content sections as needed
3. Add your own functionality to each section

### Navigation Structure

The sidebar contains navigation links that dynamically update the content area. Each link is associated with a content section using the hash in the URL.

```html
<div class="nav-item">
  <a href="#link-1" class="nav-link" data-title="Link 1">
    <!-- Icon SVG -->
    Link 1
  </a>
</div>
```

And the corresponding content section:

```html
<div class="section" id="link-1">
  <h1>Link 1 Content</h1>
  <!-- Your content here -->
</div>
```

## Customization

### Theme Customization

The template uses CSS variables for easy theming. Modify the `:root` and `[data-theme="light"]` selectors in the CSS to change colors.

```css
:root {
  --bg-primary: #0f0f0f;
  --bg-secondary: #161616;
  --sidebar-width: 12.5%;
  --header-height: 60px;
  --text-color: #ffffff;
  --accent-color: #3b82f6;
  --border-color: #2a2a2a;
  --font-family: 'Inter', sans-serif;
}

[data-theme="light"] {
  --bg-primary: #ffffff;
  --bg-secondary: #f5f5f5;
  --text-color: #333333;
  --border-color: #e0e0e0;
}
```

### Sidebar Width

Adjust the sidebar width by changing the `--sidebar-width` variable in the CSS.

### Content Layout

Add more complex layouts to each content section as needed. The content area is a simple container that can be customized with additional CSS.

## Structure

The template consists of:

- **Header**: Contains logo, page title, theme toggle, and profile
- **Sidebar**: Navigation menu with icons
- **Content Area**: Dynamic content sections that change based on navigation

## JavaScript Functionality

The template includes two main JavaScript functions:

1. `initThemeToggle()`: Handles theme switching and persistence
2. `initRouter()`: Manages navigation and content display

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This template is available for personal and commercial use.

---

**Note**: This is a starter template. You may need to extend functionality for production use.
