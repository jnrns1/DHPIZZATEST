# Drafthouse Pizza Website

A beautiful, responsive website for Drafthouse Pizza - home of the Panzoti since 1984. Built with HTML, Tailwind CSS, and deployed on Vercel.

## Features

- **Responsive Design** - Mobile-first design that works on all devices
- **Modern Styling** - Custom Tailwind CSS theme with Material Design colors
- **Performance Optimized** - Optimized caching headers and minimal dependencies
- **Analytics Ready** - Vercel Web Analytics integration

## Pages

- **Home** (`index.html`) - Hero section with weekly specials and about
- **Menu** (`menu.html`) - Digital menu
- **Locations** (`locations.html`) - Store locations
- **Reserve** (`reserve.html`) - Reservation system
- **Careers** (`careers.html`) - Job opportunities
- **Story** (`story.html`) - Company history
- **Contact** (`contact.html`) - Contact information

## Deployment

### Prerequisites
- GitHub account connected to Vercel
- Project already connected to Vercel (configured in `.vercel/project.json`)

### Deploy to Vercel

The project is configured to deploy automatically when you push to the main branch.

**Manual Deployment:**
1. Push changes to GitHub
2. Vercel will automatically detect and deploy the changes
3. Your site will be live at your Vercel domain

**Local Testing:**
```bash
# Serve the site locally to test before deployment
python -m http.server 3000
# Then visit http://localhost:3000
```

## Configuration

### `vercel.json`
- Static site hosting configuration
- URL rewrites for clean routing
- Cache control headers for performance
- Security headers (X-Frame-Options, X-Content-Type-Options)

### `.vercelignore`
- Excludes unnecessary files from deployment to keep build size minimal

### Environment Variables
The following environment variables are available:
- `VERCEL_WEB_ANALYTICS_ID` - Automatically set by Vercel for analytics

## Development

### Local Development
Simply open `index.html` in your browser or use a local server:

```bash
# Using Python 3
python -m http.server 3000

# Using Node.js (with http-server)
npx http-server -p 3000
```

### Styling
- Uses Tailwind CSS via CDN with custom theme
- Custom color palette defined in `index.html`
- Material Design icons from Google
- Custom fonts: Space Grotesk, Manrope, Plus Jakarta Sans

## Performance Optimizations

✓ Optimized cache headers for static assets
✓ Long-term caching for images, fonts, and stylesheets
✓ Minified Tailwind CSS delivery
✓ External image loading for reduced bandwidth
✓ Lazy-loaded images where appropriate

## Security

✓ X-Content-Type-Options header (prevent MIME-type sniffing)
✓ X-Frame-Options header (prevent clickjacking)
✓ Content Security Policy headers configured on Vercel

## Browser Support

Works on all modern browsers:
- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

© 2025 Drafthouse Pizza. All rights reserved.
