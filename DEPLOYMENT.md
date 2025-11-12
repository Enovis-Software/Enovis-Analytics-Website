# Deployment Guide - Enovis Analytics Website

## 🚀 Pre-Deployment Checklist

### 1. **Update Configuration Files**

#### robots.txt
- [ ] Replace `https://yourwebsite.com` with your actual domain

#### sitemap.xml
- [ ] Replace `https://yourwebsite.com` with your actual domain
- [ ] Update `<lastmod>` dates to current date

#### index.html (Meta Tags)
- [ ] Replace all `https://yourwebsite.com` with your actual domain
- [ ] Add actual social media image URLs for `og:image` and `twitter:image`
- [ ] Update canonical URL

#### JSON-LD Structured Data
- [ ] Update the organization URL in the structured data script
- [ ] Add your physical address if you have one
- [ ] Add social media profile URLs to `sameAs` array

### 2. **Test Everything Locally**

- [ ] Test on Chrome, Firefox, Safari
- [ ] Test on mobile devices
- [ ] Test all forms (contact form, assessment form)
- [ ] Test language switching (EN/RO)
- [ ] Test all internal links
- [ ] Test cookie banner functionality
- [ ] Test service modals
- [ ] Verify email links work (mailto:)
- [ ] Verify phone links work (tel:)

### 3. **Optimize Assets**

#### Optional Improvements:
- [ ] Minify CSS (`styles.css` → `styles.min.css`)
- [ ] Minify JavaScript (`script.js` → `script.min.js`)
- [ ] Create actual favicon files:
  - `favicon.ico` (16x16, 32x32)
  - `apple-touch-icon.png` (180x180)
- [ ] Create social media share images:
  - `og-image.jpg` (1200x630px for Facebook/LinkedIn)
  - `twitter-image.jpg` (1200x600px for Twitter)

### 4. **Set Up Hosting**

#### Recommended Hosting Options:

**Option A: Netlify (Easiest)**
1. Create account at [netlify.com](https://netlify.com)
2. Drag and drop your folder
3. Set up custom domain
4. SSL certificate is automatic
5. Done!

**Option B: GitHub Pages**
1. Create GitHub repository
2. Upload all files
3. Enable GitHub Pages in settings
4. Add custom domain (optional)

**Option C: Traditional Hosting (cPanel, etc.)**
1. Upload all files via FTP
2. Ensure `.htaccess` is uploaded
3. Set up SSL certificate
4. Configure domain

### 5. **Domain & DNS Configuration**

- [ ] Point your domain to hosting
- [ ] Set up A records or CNAME
- [ ] Wait for DNS propagation (24-48 hours)
- [ ] Verify domain works

### 6. **SSL Certificate**

- [ ] Install SSL certificate (Let's Encrypt is free)
- [ ] Force HTTPS (uncomment lines in `.htaccess`)
- [ ] Update all internal URLs to use `https://`
- [ ] Test SSL with [SSL Labs](https://www.ssllabs.com/ssltest/)

### 7. **Post-Deployment**

#### Immediate Actions:
- [ ] Submit sitemap to Google Search Console
- [ ] Submit sitemap to Bing Webmaster Tools
- [ ] Verify Google Forms work correctly
- [ ] Test contact email and phone links
- [ ] Check all pages load correctly

#### Analytics Setup (Optional):
- [ ] Set up Google Analytics 4
- [ ] Add GA4 tracking code to all pages
- [ ] Set up conversion tracking for form submissions
- [ ] Configure goals and events

#### Social Media:
- [ ] Test how links appear when shared on Facebook
- [ ] Test how links appear when shared on LinkedIn
- [ ] Test how links appear when shared on Twitter
- [ ] Use [Facebook Debugger](https://developers.facebook.com/tools/debug/)

### 8. **SEO Setup**

- [ ] Google Search Console: Add and verify property
- [ ] Submit sitemap
- [ ] Request indexing for main pages
- [ ] Bing Webmaster Tools: Add and verify
- [ ] Set up Google Business Profile (if applicable)

### 9. **Performance Testing**

Test your site with:
- [ ] [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [ ] [GTmetrix](https://gtmetrix.com/)
- [ ] [WebPageTest](https://www.webpagetest.org/)

Target Scores:
- PageSpeed: 90+ (mobile and desktop)
- GTmetrix: A grade
- First Contentful Paint: < 1.5s

### 10. **Security Testing**

- [ ] Test SSL configuration
- [ ] Check security headers with [SecurityHeaders.com](https://securityheaders.com/)
- [ ] Verify cookie policy is displayed
- [ ] Test GDPR compliance

## 📁 Files to Upload

**Required Files:**
```
index.html
styles.css
script.js
translations.json
privacy-policy.html
terms-of-service.html
cookie-policy.html
404.html
robots.txt
sitemap.xml
favicon.svg
.htaccess (for Apache servers)
```

**Optional but Recommended:**
```
favicon.ico
apple-touch-icon.png
og-image.jpg
twitter-image.jpg
```

## 🔧 Server Requirements

**Minimum:**
- PHP: Not required (static HTML)
- Web Server: Apache, Nginx, or any static hosting
- HTTPS/SSL: Required for production
- Storage: < 1 MB

**Recommended Server Configuration:**
- Enable gzip compression
- Enable browser caching
- Set up proper MIME types
- Configure security headers

## 🌍 Domain Updates Needed

After deployment, search and replace in these files:

1. **robots.txt**: Line 9
2. **sitemap.xml**: All `<loc>` tags
3. **index.html**: Lines 13-25 (meta tags)
4. **index.html**: Lines 397, 407 (JSON-LD)

Replace `https://yourwebsite.com` with your actual domain.

## 📊 Monitoring

### Uptime Monitoring (Optional):
- [UptimeRobot](https://uptimerobot.com/) (Free)
- [Pingdom](https://www.pingdom.com/)

### Analytics (Optional):
- Google Analytics 4
- Microsoft Clarity
- Hotjar

## 🆘 Troubleshooting

### Common Issues:

**Issue: 404 Error on all pages**
- Solution: Ensure `.htaccess` is uploaded (if using Apache)

**Issue: Google Form not loading**
- Solution: Check Content Security Policy headers
- Ensure `https://docs.google.com` is allowed

**Issue: Cookie banner not appearing**
- Solution: Clear browser localStorage and test in incognito

**Issue: CSS not loading**
- Solution: Check file paths are correct
- Clear browser cache

**Issue: Language switching not working**
- Solution: Check `translations.json` is uploaded
- Check browser console for errors

## 📞 Support Resources

- **Web Hosting Support**: Contact your hosting provider
- **Domain Issues**: Contact your domain registrar
- **Technical Issues**: Check browser console (F12)

## ✅ Final Checklist

- [ ] All URLs updated to production domain
- [ ] SSL certificate installed and working
- [ ] All forms tested and working
- [ ] Analytics tracking code added (if using)
- [ ] Sitemap submitted to search engines
- [ ] Social media sharing tested
- [ ] Mobile responsiveness verified
- [ ] All legal pages accessible
- [ ] Cookie consent working
- [ ] Contact information verified
- [ ] Backup of all files created

---

**🎉 Your website is ready for launch!**

For updates or issues, refer to this guide or contact your web administrator.

