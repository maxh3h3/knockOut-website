# knockOut Study - Website

A modern, responsive static website for the knockOut Study language learning application.

## 🌟 Overview

This repository contains the official website for knockOut Study, featuring:
- Landing page with app showcase
- CTO recruitment page (bilingual EN/RU)
- Comprehensive support documentation
- Privacy policy
- Custom 404 error page

## 📁 Project Structure

```
kO_Website_Pages/
├── index.html              # Main landing page
├── cto.html                # CTO recruitment page (bilingual)
├── support.html            # Support and FAQ page
├── privacy-policy.html     # Privacy policy
├── 404.html               # Custom error page
├── robots.txt             # Search engine directives
├── sitemap.xml            # Site structure for SEO
├── .htaccess              # Apache server configuration
├── assets/                # Images and media files
│   ├── app_icon.png
│   ├── main logo.png
│   ├── Textlogo.png
│   └── screenshots/       # App screenshots
└── README.md              # This file
```

## 🚀 Features

### 🎨 Design & User Experience
- **Responsive Design**: Mobile-first approach with perfect scaling across all devices
- **Modern UI**: Clean, professional design with smooth animations
- **Consistent Navigation**: Unified header navigation across all pages
- **Accessibility**: Proper semantic HTML and ARIA labels
- **Fast Loading**: Optimized images and efficient CSS

### 🔍 SEO Optimized
- **Meta Tags**: Comprehensive meta descriptions and Open Graph tags
- **Structured Data**: Search engine friendly markup
- **Sitemap**: XML sitemap for search engine indexing
- **Robots.txt**: Proper search engine directives
- **Clean URLs**: SEO-friendly URL structure

### 🛡️ Security & Performance
- **Security Headers**: XSS protection, MIME sniffing prevention
- **GZIP Compression**: Faster page loading
- **Browser Caching**: Optimized cache settings
- **Content Security Policy**: Basic CSP implementation

### 🌐 Multilingual Support
- **Bilingual CTO Page**: English/Russian language toggle
- **Smooth Transitions**: JavaScript-powered language switching
- **Consistent Experience**: Maintained design across languages

## 🚀 Deployment

### Option 1: Static Hosting (Recommended)

#### Netlify
1. Connect your GitHub repository to Netlify
2. Set build command: `# No build required for static site`
3. Set publish directory: `/`
4. Deploy automatically on git push

#### Vercel
1. Import project from GitHub
2. Framework preset: `Other`
3. Build command: Leave empty
4. Output directory: `./`
5. Deploy

#### GitHub Pages
1. Go to repository Settings > Pages
2. Source: Deploy from branch
3. Branch: `main` or `master`
4. Folder: `/ (root)`
5. Save

### Option 2: Traditional Web Hosting

#### Requirements
- Apache or Nginx web server
- PHP not required (static HTML)
- HTTPS recommended for production

#### Upload Files
1. Upload all files to your web server's public directory
2. Ensure `.htaccess` is uploaded (may be hidden)
3. Update `sitemap.xml` with your actual domain
4. Update `robots.txt` with your domain

### Option 3: Docker (Optional)

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

```bash
docker build -t knockout-website .
docker run -p 80:80 knockout-website
```

## 🔧 Configuration

### Before Deployment

1. **Update Domain References**:
   - Replace `https://yourdomain.com` in `sitemap.xml` with your actual domain
   - Update `robots.txt` with your domain
   - Update canonical URLs in HTML meta tags

2. **Analytics Setup** (Optional):
   - Add Google Analytics tracking code
   - Set up Google Search Console
   - Configure any other tracking tools

3. **Security (Production)**:
   - Uncomment HTTPS redirect in `.htaccess`
   - Enable HSTS headers for HTTPS
   - Review and adjust Content Security Policy

### Customization

#### Colors & Branding
- Primary color: `#667eea` (Purple gradient start)
- Secondary color: `#764ba2` (Purple gradient end)
- Accent color: `#ff6b6b` (Red for CTAs)
- Orange accent: `#ff7f00` (Support pages)

#### Content Updates
- Update contact email (`maxx.hamad@gmail.com`) across all pages
- Modify app store links when available
- Update company information
- Adjust privacy policy as needed

## 📱 Mobile Optimization

- Fully responsive design
- Touch-friendly navigation
- Optimized image sizes for mobile
- Fast loading on slow connections
- Mobile-first CSS approach

## 🔍 SEO Checklist

✅ Meta descriptions on all pages  
✅ Open Graph tags for social sharing  
✅ Proper heading hierarchy (H1, H2, H3)  
✅ Alt text for all images  
✅ Internal linking structure  
✅ XML sitemap  
✅ Robots.txt  
✅ Fast loading times  
✅ Mobile-friendly design  
✅ HTTPS ready  

## 🛠️ Development

### Local Development
1. Clone the repository
2. Open in your preferred editor
3. Use a local server for testing:
   ```bash
   # Python
   python -m http.server 8000
   
   # Node.js
   npx serve .
   
   # PHP
   php -S localhost:8000
   ```
4. Navigate to `http://localhost:8000`

### File Structure Guidelines
- Keep all images in `/assets/`
- Maintain consistent CSS patterns
- Use semantic HTML elements
- Follow responsive design principles
- Test on multiple devices and browsers

## 📊 Performance

### Core Web Vitals Targets
- **LCP (Largest Contentful Paint)**: < 2.5s
- **FID (First Input Delay)**: < 100ms
- **CLS (Cumulative Layout Shift)**: < 0.1

### Optimization Features
- Compressed images (recommend WebP when possible)
- Minified CSS (embedded for fewer requests)
- Efficient font loading (Google Fonts)
- Lazy loading for images (implement if needed)

## 🔗 External Links

Update these when available:
- App Store link
- Google Play Store link
- TestFlight link
- Social media profiles

## 📞 Support

For technical issues with the website:
- Email: maxx.hamad@gmail.com
- Create an issue in this repository

## 📄 License

This website code is proprietary to knockOut Study. All rights reserved.

---

**Last Updated**: January 2025  
**Version**: 1.0.0  
**Maintainer**: knockOut Study Team
