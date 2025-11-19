# Will Spark Media - Website

A modern, creative website for Will Spark Media showcasing digital marketing services.

## Features

- Modern, creative design with smooth animations
- Fully responsive layout (mobile, tablet, desktop)
- Interactive elements with tilt effects and parallax
- Optimized for performance
- SEO-friendly structure
- Accessible design
- Ready for Cloudflare Pages deployment

## Tech Stack

- HTML5
- CSS3 (Custom properties, Grid, Flexbox)
- Vanilla JavaScript (ES6+)
- Google Fonts (Inter & Space Grotesk)

## Project Structure

```
WillSparkMedia/
├── index.html          # Main HTML file
├── styles.css          # All CSS styling
├── script.js           # JavaScript functionality
├── wrangler.toml       # Cloudflare configuration
└── README.md           # Documentation
```

## Deploying to Cloudflare Pages

### Option 1: Git Integration (Recommended)

1. Push your code to GitHub/GitLab
2. Log in to [Cloudflare Dashboard](https://dash.cloudflare.com/)
3. Go to **Pages** > **Create a project**
4. Connect your Git repository
5. Configure build settings:
   - **Build command**: (leave empty)
   - **Build output directory**: `/`
   - **Root directory**: `/`
6. Click **Save and Deploy**

### Option 2: Direct Upload

1. Log in to [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. Go to **Pages** > **Create a project** > **Direct upload**
3. Upload your project folder (index.html, styles.css, script.js)
4. Click **Deploy site**

### Option 3: Wrangler CLI

```bash
# Install Wrangler globally
npm install -g wrangler

# Login to Cloudflare
wrangler login

# Deploy to Cloudflare Pages
wrangler pages deploy . --project-name=willsparkmedia
```

## Local Development

Simply open `index.html` in your browser, or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Customization

### Colors

Edit CSS variables in `styles.css`:

```css
:root {
    --primary: #4169E1;
    --secondary: #FF6B9D;
    --accent: #FFD93D;
    /* ... more colors */
}
```

### Content

- Update text content directly in `index.html`
- Replace placeholder images with real images
- Modify services, portfolio items, and contact information

### Form Submission

The contact form currently has a simulated submission. To connect it to a real backend:

1. Update the form handling in `script.js` (line ~180)
2. Options:
   - Use Cloudflare Workers for serverless backend
   - Connect to form services like Formspree, Netlify Forms, or Basin
   - Set up your own API endpoint

Example with Formspree:

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## Performance Optimizations

- Minify CSS and JavaScript for production
- Optimize and compress images
- Use WebP format for images
- Enable Cloudflare's auto-minify features

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome)

## Contact

For questions or issues, contact Will Spark Media:
- Phone: 017-795 1130
- Email: info@YaWillSpark.media

## License

Copyright 2025 Will Spark Media. All rights reserved.