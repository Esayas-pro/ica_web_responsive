# ICA Web Responsive

A comprehensive responsive web interface module for Odoo 17.0 that enhances the user experience with modern UI/UX improvements and dark mode support.

## Overview

ICA Web Responsive transforms Odoo's web interface into a fully responsive, modern application with enhanced usability across all devices. Developed by IdeaCode Academy, this module provides a seamless experience on desktop, tablet, and mobile devices.

## Features

### Core Features
- **Fully Responsive Design** - Adaptive layouts for all screen sizes
- **Dark Mode Support** - Complete dark theme implementation with automatic switching
- **Enhanced Navigation** - Improved navbar and menu system
- **Mobile Optimized** - Touch-friendly interface for mobile devices
- **Bootstrap Overrides** - Custom styling for better visual consistency

### UI Components
- Responsive home menu with custom backgrounds
- Improved list views for desktop and mobile
- Enhanced pivot table views
- Modernized navbar with better accessibility
- Optimized form layouts for smaller screens

## Installation

1. **Copy the module to your Odoo addons directory:**
```bash
cp -r ica_web_responsive /path/to/odoo/custom_addons/
```

2. **Update the module list:**
   - Navigate to Apps menu in Odoo
   - Click "Update Apps List"
   - Search for "ICA Responsive"

3. **Install the module:**
   - Click Install on the ICA Responsive module
   - Wait for the installation to complete

## Configuration

The module works out of the box with minimal configuration:

### Dark Mode
- Dark mode assets are automatically loaded based on user preference
- Users can toggle between light and dark themes
- Persistent theme selection across sessions

### Responsive Breakpoints
Default breakpoints are optimized for:
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

## Technical Details

### Dependencies
- `web` - Odoo web client
- `base_setup` - Base setup module

### Assets Structure
```
static/
├── src/
│   ├── core/           # Core functionality
│   ├── scss/           # SCSS variables and overrides
│   ├── views/          # View-specific enhancements
│   │   ├── list/       # List view improvements
│   │   └── pivot/      # Pivot table enhancements
│   └── webclient/      # Web client components
│       ├── home_menu/  # Home menu customizations
│       └── navbar/     # Navigation bar improvements
├── description/        # Module images and descriptions
└── img/               # Additional images
```

### Key Files
- `__manifest__.py` - Module configuration and asset definitions
- `views/webclient_templates.xml` - XML templates for web client
- `static/src/main.js` - Main JavaScript entry point
- `static/src/scss/primary_variables.scss` - Primary theme variables
- `static/src/scss/bootstrap_overridden.scss` - Bootstrap customizations

## Customization

### Modifying Theme Colors
Edit the SCSS variables in:
- Light mode: `static/src/scss/primary_variables.scss`
- Dark mode: `static/src/scss/primary_variables.dark.scss`

### Adding Custom Responsive Rules
Add your custom SCSS in:
```scss
static/src/webclient/your_component/your_component.scss
```

### Extending JavaScript Functionality
Create new components in:
```javascript
static/src/webclient/your_component/your_component.js
```

## Compatibility

- **Odoo Version:** 17.0+
- **Browsers:** Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile:** iOS Safari, Chrome Mobile, Android Browser

## Known Issues

- Pivot tables may require horizontal scrolling on very small screens
- Some third-party modules may require additional responsive adjustments

## Support

For issues, questions, or contributions:
- **Author:** Agga, IdeaCode Academy
- **License:** LGPL-3

## Changelog

### Version 1.0
- Initial release
- Full responsive design implementation
- Dark mode support
- Mobile navigation improvements
- Bootstrap integration

## Screenshots

Module includes demo images in `static/description/` directory showing the responsive interface in action.

---

*Developed by IdeaCode Academy - Making Odoo more accessible and user-friendly*
