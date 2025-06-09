# Dashboard Project

A responsive web dashboard built with HTML and CSS featuring a modern grid-based layout.

## Overview

This project is a clean, professional dashboard interface that demonstrates modern CSS Grid and Flexbox techniques. It features a sidebar navigation, header with search functionality, project cards grid, and informational panels.

## Features

### Layout Structure
- **Responsive Grid Layout**: Uses CSS Grid for the main layout structure
- **Sidebar Navigation**: Fixed sidebar with dashboard branding and navigation links
- **Header Bar**: Top header with search functionality and user options
- **Main Content Area**: Project cards displayed in a responsive grid
- **Right Panel**: Announcements and trending sections

### Components

#### Sidebar
- Dashboard logo and title
- Navigation menu with icons:
  - Home
  - Profile
  - Messages
  - History
  - Tasks
  - Communities
- Settings section:
  - Settings
  - Support
  - Privacy

#### Header
- **Top Header**:
  - Search bar with search button
  - Notification bell
  - User profile icon
  - Username display
- **Bottom Header**:
  - User greeting section with profile picture
  - Action buttons (Post, Upload, Share)

#### Main Content
- **Projects Section**: Grid of project cards with:
  - Project title and description
  - Action buttons (Star, Watch, Fork)
- **Announcements Panel**: List of site announcements
- **Trending Panel**: Trending users and content

## File Structure

```
dashboard/
├── index.html          # Main HTML structure
├── style.css           # All styling and layout
├── README.md           # This file
└── resources/          # SVG icons
    ├── account-circle.svg
    ├── account-group.svg
    ├── bell-ring.svg
    ├── calendar-check.svg
    ├── cctv.svg
    ├── cog.svg
    ├── Dashboard.svg
    ├── fork.svg
    ├── history.svg
    ├── home-circle.svg
    ├── magnify.svg
    ├── message.svg
    ├── star.svg
    ├── tooltip-question.svg
    └── watch.svg
```

## Technical Details

### CSS Techniques Used
- **CSS Grid**: Main layout structure with `grid-template-columns` and `grid-template-rows`
- **Flexbox**: Component-level layouts for headers, cards, and navigation
- **Responsive Design**: Uses `clamp()` function for responsive sizing
- **CSS Variables**: Color scheme with teal accents and blue sidebar
- **Modern Selectors**: First-child and last-child pseudo-selectors for styling

### Layout Specifications
- **Viewport Height**: Full viewport height (`100vh`) layout
- **Grid Proportions**: 
  - Columns: `0.7fr 4fr` (sidebar to main content ratio)
  - Rows: `0.2fr 1fr` (header to content ratio)
- **Color Scheme**:
  - Sidebar: Blue (`rgb(70, 150, 242)`)
  - Background: Light gray
  - Cards: White with subtle shadows
  - Accent: Teal buttons

### Browser Compatibility
- Modern browsers supporting CSS Grid and Flexbox
- Uses modern CSS functions like `clamp()` and `calc()`

## Usage

1. Open `index.html` in a web browser
2. The dashboard will display with:
   - Functional layout (styling only, no JavaScript functionality)
   - Responsive design that adapts to different screen sizes
   - Interactive hover states on buttons and navigation items

## Customization

### Adding New Projects
Add new project cards in the `.projectBoard` section of `index.html`:

```html
<div class="card">
    <h4>Project Name</h4>
    <p>Project description...</p>
    <div class="cardButtons">
        <button class="cardBtn"><img src="resources/star.svg" alt="Star"></button>
        <button class="cardBtn"><img src="resources/watch.svg" alt="Watch"></button>
        <button class="cardBtn"><img src="resources/fork.svg" alt="Fork"></button>
    </div>
</div>
```

### Modifying Colors
Key color variables in `style.css`:
- Sidebar background: `rgb(70, 150, 242)`
- Button accent: `teal`
- Background: `lightgray`
- Cards: `white`

### Adding Icons
Place new SVG icons in the `resources/` folder and reference them in the HTML.

## Future Enhancements

- Add JavaScript functionality for interactive features
- Implement responsive breakpoints for mobile devices
- Add dark/light theme toggle
- Connect to backend APIs for dynamic content
- Add user authentication and personalization

## Credits

Built as part of The Odin Project curriculum to practice CSS Grid and modern layout techniques.
