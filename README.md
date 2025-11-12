# Enovis Analytics - Business Intelligence Website

A modern, production-ready presentation website for business intelligence and data analysis services. Built with vanilla JavaScript, HTML, and CSS - no frameworks required.

**🚀 PRODUCTION READY** - Fully optimized for deployment with SEO, security, and legal compliance built-in.

## Features

✨ **Modern Design**
- Apple-inspired fluid design with blue color palette
- Minimalist and clear interface
- Smooth animations and transitions
- Fully responsive (mobile, tablet, desktop)

🌍 **Multi-language Support**
- English and Romanian translations
- Auto-detection based on browser language
- Manual language switcher
- All text stored in `translations.json` for easy editing

📊 **Services Showcase**
- Data Streams & Sources
- Data Centralization & Transformation
- ETL Pipelines
- Interactive Dashboards
- Data Insights & Analytics
- Forecasting & Predictions

📱 **Responsive Design**
- Optimized for all screen sizes
- Touch-friendly navigation
- Mobile-first approach

## Quick Start

1. **Open the website**: Simply open `index.html` in your browser
2. **Test language switching**: Click EN/RO buttons in the navigation
3. **Integrate Google Form**: Follow instructions below

## Google Form Integration

To add your contact form:

1. Create a Google Form at [forms.google.com](https://forms.google.com)
2. Click **Send** button
3. Select the **<> Embed HTML** tab
4. Copy the URL from the `src` attribute
5. Open `index.html` and find this line (around line 158):

```html
<iframe 
    src="https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform?embedded=true"
```

6. Replace `YOUR_FORM_ID` with your actual form ID

### Example
If your embed code looks like:
```html
<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdXXXXXX/viewform?embedded=true">
```

Use: `1FAIpQLSdXXXXXX` as your form ID

## Customization

### Changing Colors

Edit `styles.css` and modify the CSS variables at the top:

```css
:root {
    --primary-blue: #007AFF;
    --secondary-blue: #0051D5;
    --light-blue: #5AC8FA;
    /* Add more customizations here */
}
```

### Adding/Editing Translations

Edit `translations.json`:

```json
{
  "en": {
    "hero": {
      "title": "Your Custom Title"
    }
  },
  "ro": {
    "hero": {
      "title": "Titlul Tău Personalizat"
    }
  }
}
```

### Changing Content

All text is marked with `data-i18n` attributes. To change text:
1. Find the element in `index.html`
2. Note the `data-i18n` value (e.g., `data-i18n="hero.title"`)
3. Update the corresponding text in `translations.json`

### Adding New Services

In `index.html`, add a new service card in the `.services-grid` section:

```html
<div class="service-card">
    <div class="service-icon">
        <!-- Add your SVG icon here -->
    </div>
    <h3 class="service-title" data-i18n="services.newService.title">Service Title</h3>
    <p class="service-description" data-i18n="services.newService.description">Description</p>
</div>
```

Then add translations to `translations.json`:

```json
"services": {
    "newService": {
        "title": "New Service",
        "description": "Service description"
    }
}
```

## File Structure

```
Website/
│
├── index.html              # Main homepage
├── styles.css              # All styling and design
├── script.js               # JavaScript functionality
├── translations.json       # Language translations (EN/RO)
│
├── privacy-policy.html     # GDPR-compliant privacy policy
├── terms-of-service.html   # Terms and conditions
├── cookie-policy.html      # Cookie usage policy
├── 404.html               # Custom error page
│
├── robots.txt             # Search engine instructions
├── sitemap.xml            # SEO sitemap
├── favicon.svg            # Website icon
├── .htaccess              # Apache server configuration
│
├── DEPLOYMENT.md          # Deployment guide
└── README.md              # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Production Features

### Performance
- ⚡ Fast loading - no external dependencies
- 🎯 SEO optimized with meta tags and structured data
- ♿ Accessible design (semantic HTML)
- 🔒 Secure (no external scripts except Google Forms)
- 📦 Lightweight (< 1 MB total)

### SEO & Marketing
- ✅ Complete meta tags (Open Graph, Twitter Cards)
- ✅ JSON-LD structured data for search engines
- ✅ Sitemap.xml for search engine indexing
- ✅ Robots.txt for crawler management
- ✅ Canonical URLs
- ✅ Multi-language hreflang tags

### Legal Compliance
- ✅ GDPR-compliant cookie consent banner
- ✅ Comprehensive privacy policy
- ✅ Terms of service
- ✅ Cookie policy
- ✅ User rights management (GDPR)

### Security
- ✅ Security headers configured (.htaccess)
- ✅ XSS protection
- ✅ Clickjacking prevention
- ✅ Content Security Policy
- ✅ HTTPS-ready

### User Experience
- ✅ Custom 404 error page
- ✅ Service detail modals
- ✅ Contact forms (Google Forms integration)
- ✅ BI maturity self-assessment
- ✅ Smooth animations and transitions

## Deployment

**See [DEPLOYMENT.md](DEPLOYMENT.md) for complete deployment instructions.**

### Quick Start

1. **Update Configuration**
   - Replace `https://yourwebsite.com` with your actual domain in:
     - `robots.txt`
     - `sitemap.xml`
     - `index.html` (meta tags and JSON-LD)

2. **Upload Files**
   - Upload all files to your hosting
   - Ensure `.htaccess` is uploaded (Apache servers)

3. **Set Up SSL**
   - Install SSL certificate (free with Let's Encrypt)
   - Force HTTPS in `.htaccess`

4. **Submit to Search Engines**
   - Submit `sitemap.xml` to Google Search Console
   - Submit to Bing Webmaster Tools

### Hosting Options

**Recommended:** Netlify, Vercel, or GitHub Pages (easiest)
**Traditional:** Any hosting with Apache/Nginx support

## Best Practices Implemented

✅ **Design**
- Consistent spacing and typography
- Clear visual hierarchy
- Accessible color contrasts
- Smooth, subtle animations

✅ **Code Quality**
- Semantic HTML5
- Modern CSS with CSS variables
- Clean, commented JavaScript
- Mobile-first responsive design

✅ **Performance**
- Minimal HTTP requests
- Optimized animations
- Efficient JavaScript
- No external dependencies

✅ **UX**
- Clear call-to-actions
- Easy navigation
- Fast page loads
- Intuitive interface

## Customization Tips

1. **Logo**: Replace "Enovis Analytics Data" text with your own logo/image
2. **Colors**: Use the CSS variables for consistent theming
3. **Fonts**: Change `--font-system` in CSS to use custom fonts
4. **Contact Info**: Update email in the contact section
5. **Meta Tags**: Update title and description in `<head>` for SEO

## Support

For questions or issues:
- Review this README
- Check `translations.json` for text changes
- Inspect `styles.css` for design modifications
- Review `script.js` for functionality

## License

Free to use for personal and commercial projects.

---

Built with ❤️ using vanilla HTML, CSS, and JavaScript

