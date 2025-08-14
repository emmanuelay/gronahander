# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the website for "Gröna Händer" (Green Hands), a Swedish gardening and home services business based in Göteborg. The site is built using a customized Bootstrap HTML template and focuses on services like lawn mowing, garden bed maintenance, window cleaning, and custom gardening work.

## Architecture

### Static Website Structure
- **Frontend**: Pure HTML/CSS/JavaScript static website
- **Template**: Bootstrap-based gardening template from HTML Codex
- **Hosting**: GitHub Pages (indicated by CNAME file)
- **Language**: Swedish (primary content language)

### Key Files
- `index.html` - Main homepage with services, projects, and booking information
- `team.html` - Team page (template content, not customized)
- `404.html` - Error page (template content, not customized)
- `css/style.css` - Main stylesheet with custom styling
- `css/bootstrap.min.css` - Bootstrap framework styles
- `js/main.js` - Main JavaScript for interactions and animations
- `scss/bootstrap.scss` - SCSS source for Bootstrap customization

### Third-Party Libraries
- **Bootstrap 5.0.0** - UI framework
- **jQuery 3.4.1** - DOM manipulation
- **WOW.js** - Scroll animations
- **Owl Carousel** - Testimonial carousel
- **Lightbox** - Image gallery
- **Isotope** - Portfolio filtering
- **CounterUp** - Number animations
- **Parallax** - Parallax scrolling effects

### Design System
- **Primary Color**: #348E38 (green)
- **Secondary Color**: #525368 (gray)
- **Light Color**: #E8F5E9 (light green)
- **Dark Color**: #0F4229 (dark green)
- **Fonts**: 'Jost' for headings, 'Open Sans' for body text

## Development Workflow

### No Build Process
This is a static HTML website with no build step. CSS and JavaScript are served directly or from CDN.

### File Serving
- Open `index.html` directly in browser for local development
- All assets are relative paths or CDN links

### CSS Compilation (Optional)
If modifying SCSS files:
```bash
# Compile SCSS to CSS (requires Sass compiler)
sass scss/bootstrap.scss css/bootstrap.min.css --style compressed
```

### Testing
- Open files directly in browser
- Test responsive design at different screen sizes
- Verify external links (Calendly booking, social media)

## Business Context

### Services Offered
- **Gräsklippning** - Lawn mowing
- **Rabattrensning** - Garden bed cleaning
- **Fönsterputs** - Window cleaning
- **Övrigt** - Custom services

### Key Business Information
- **Phone**: +46 70-485 42 71
- **Location**: Göteborg, Sweden
- **Booking**: Via Calendly integration
- **Social Media**: TikTok (@grona_hander), Instagram (@gronahander_hemtjanst)

### Important URLs
- **Booking Link**: https://calendly.com/ruben-c101019/grona-hander
- **TikTok**: https://www.tiktok.com/@grona_hander
- **Instagram**: https://www.instagram.com/gronahander_hemtjanst/

## File Structure Notes

### Content vs Template
- `index.html` - Fully customized with Swedish content and branding
- `team.html` and `404.html` - Still contain template placeholder content
- Template attribution preserved in footer as required by license

### Image Assets
- Service images in `img/service-*.jpg`
- Carousel images in `img/carousel-*.jpg`
- Icons in `img/icon/` directory
- Logo/favicon: `img/grönahänder.png`

### Library Files
- All third-party libraries stored locally in `lib/` directory
- Bootstrap source SCSS files included for customization

## Common Tasks

### Content Updates
- Edit HTML files directly
- Update contact information, services, or business details
- Modify booking links or social media URLs

### Styling Changes
- Edit `css/style.css` for custom styles
- Modify `scss/bootstrap.scss` for theme colors and compile if needed
- Update CSS custom properties in `:root` for color scheme changes

### Adding New Services
- Add service card in the services section of `index.html`
- Add corresponding image in `img/` directory
- Update portfolio/projects section if needed