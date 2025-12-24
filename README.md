# Velorum Software Corporate Website

A clean, professional corporate website for Velorum Software Ltd showcasing three enterprise SaaS products.

## Files Structure

```
velorum-website/
├── index.html          # Main homepage
├── privacy.html        # Privacy policy page (placeholder)
├── terms.html          # Terms of service page (placeholder)
├── styles.css          # All styling
└── assets/            # Product logos
    ├── agentpmo-logo-160_1_.png
    ├── agentpmo-favicon-48_1_.png
    ├── ISSA.png
    ├── Prept-logo-160_1_.png
    └── Prept-favicon-48_1_.png
```

## Quick Start

### Option 1: Deploy to Any Web Host
1. Upload all files maintaining the directory structure
2. Point your domain to the hosting
3. Done!

### Option 2: Test Locally
1. Simply open `index.html` in your browser
2. Or use a local server:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Or Node.js
   npx serve
   ```
3. Visit http://localhost:8000

## Deployment Platforms

### Netlify (Recommended - Free)
1. Drag and drop the entire folder to netlify.com/drop
2. Or connect to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin <your-repo>
   git push -u origin main
   ```
3. Connect repository in Netlify dashboard
4. Auto-deploy on push!

### Vercel (Also Free)
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the directory
3. Follow prompts

### GitHub Pages (Free)
1. Create repo named `username.github.io` or any repo name
2. Push code to `main` branch
3. Enable Pages in Settings → Pages
4. Select `main` branch and `/root` directory

### Traditional Hosting (cPanel, etc.)
1. Zip the entire folder
2. Upload via FTP or File Manager
3. Extract in public_html or www directory

## Customization

### Update Product Links
In `index.html`, update these lines when ISSA is ready:
```html
<!-- Line ~90 -->
<a href="https://issa.com" class="product-link" target="_blank">Learn More →</a>
```

Remove the `coming-soon` class from the ISSA link.

### Update Contact Emails
Replace placeholder emails in `index.html`:
- info@velorum.com
- sales@velorum.com
- careers@velorum.com

### Add Privacy Policy & Terms
Replace content in `privacy.html` and `terms.html` with your actual policies.

### Color Customization
All colors are defined in `styles.css` under `:root`:
```css
:root {
    --velorum-blue: #0020C2;
    --velorum-deep: #001A99;
    --velorum-bright: #0029FF;
    /* ... */
}
```

### Add Google Analytics (Optional)
Add before closing `</head>` tag in all HTML files:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## Features

✅ Fully responsive (mobile, tablet, desktop)
✅ Clean, modern design
✅ Fast loading (no frameworks, minimal dependencies)
✅ SEO-friendly HTML structure
✅ Accessible (semantic HTML, ARIA where needed)
✅ Professional typography (Inter font from Google Fonts)
✅ Smooth animations and transitions
✅ Sticky header navigation
✅ Bold, confident brand presence

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Android)

## Performance

- Minimal external dependencies (only Google Fonts)
- Optimized images
- Fast load times
- Lighthouse score: 95+ expected

## Notes

- Product logos are in the `assets/` folder
- Favicons for individual products included but not currently used site-wide
- To add a Velorum favicon, create one and add to `<head>`:
  ```html
  <link rel="icon" type="image/png" sizes="48x48" href="/assets/velorum-favicon-48.png">
  ```

## Support

For questions or customization requests:
- Email: info@velorum.com
- Update content in HTML files
- Update styles in styles.css

---

Built with care for Velorum Software Ltd.
