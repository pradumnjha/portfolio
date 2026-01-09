# Pradumn Jha - Professional Portfolio Website

A modern, responsive portfolio website for DevOps and SRE professionals. Built with HTML5, CSS3, and vanilla JavaScript.

## Features

✅ **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
✅ **Modern UI** - Clean, professional design with smooth animations
✅ **Multiple Sections** - Home, About, Experience, Skills, Projects, Certifications, Contact
✅ **Smooth Scrolling** - Navigation links with smooth page scrolling
✅ **Interactive Elements** - Hover effects, animations, and transitions
✅ **Dark/Light Theme** - Responsive to system color scheme preferences
✅ **Contact Form** - Ready-to-integrate contact form
✅ **SEO Friendly** - Proper semantic HTML structure

## File Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Customization Guide

### 1. **Personal Information**
Update the following in `index.html`:

- **Name**: Replace "Pradumn Jha" with your name
- **Email**: Update `your-email@example.com` in the Contact section
- **Phone**: Update `+91 98765 43210` with your phone number
- **Location**: Replace "Your City, Country" with your actual location
- **Social Links**: Update LinkedIn, GitHub, and Twitter URLs

### 2. **Professional Experience**
Edit the Experience section in `index.html`:

```html
<div class="timeline-item">
    <div class="timeline-date">YEAR - YEAR</div>
    <div class="timeline-content">
        <h3>Your Job Title</h3>
        <p class="company">Your Company Name</p>
        <ul class="achievements">
            <li>Your achievement 1</li>
            <li>Your achievement 2</li>
            <li>Your achievement 3</li>
        </ul>
    </div>
</div>
```

### 3. **Technical Skills**
Modify the Skills section with your technologies:

```html
<div class="skill-category">
    <h3>Your Skill Category</h3>
    <div class="skill-tags">
        <span class="tag">Skill 1</span>
        <span class="tag">Skill 2</span>
        <span class="tag">Skill 3</span>
    </div>
</div>
```

### 4. **Projects**
Update the Projects section with your actual projects:

```html
<div class="project-card">
    <div class="project-header">
        <h3>Your Project Title</h3>
        <div class="project-tags">
            <span class="tag-small">Technology1</span>
            <span class="tag-small">Technology2</span>
        </div>
    </div>
    <p>Project description...</p>
    <ul class="project-highlights">
        <li>Achievement 1</li>
        <li>Achievement 2</li>
    </ul>
    <a href="project-link.html" class="project-link">Learn More →</a>
</div>
```

### 5. **Certifications**
Update your certifications:

```html
<div class="cert-card">
    <i class="fas fa-certificate"></i>
    <h3>Your Certification Name</h3>
    <p>Issuing Organization</p>
    <span class="cert-year">2024</span>
</div>
```

### 6. **Statistics**
Update the about section stats (6 years, 50+ projects, etc.):

```html
<div class="stat">
    <h3>10+</h3>
    <p>Your Stat Label</p>
</div>
```

## Color Customization

Edit the CSS variables in `styles.css` (lines 8-16):

```css
:root {
    --primary-color: #0066cc;      /* Main blue */
    --secondary-color: #00a8e8;    /* Light blue */
    --accent-color: #ff6b6b;       /* Red accent */
    --dark-bg: #0a0e27;            /* Dark background */
    --light-bg: #f5f7fa;           /* Light background */
    --card-bg: #ffffff;            /* Card background */
    --text-dark: #1a1a1a;          /* Dark text */
    --text-light: #666666;         /* Light text */
}
```

## Font Customization

To change the font, update the `font-family` in `styles.css`:

```css
body {
    font-family: 'Your Font Name', fallback, sans-serif;
}
```

Popular font families:
- `'Inter', sans-serif`
- `'Poppins', sans-serif`
- `'Roboto', sans-serif`
- `'Playfair Display', serif` (for heading fonts)

## Adding Google Fonts

Add this link in the `<head>` of `index.html` before the `styles.css` link:

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

Then update the `body` font-family in `styles.css`.

## Contact Form Integration

To make the contact form functional, you have several options:

### Option 1: Email Service (Recommended)
Use EmailJS or similar service:

```javascript
// Add this to script.js
emailjs.init('your_public_key');

contactForm.addEventListener('submit', function(e) {
    e.preventDefault();
    emailjs.sendForm('service_id', 'template_id', this).then(() => {
        alert('Message sent successfully!');
        this.reset();
    });
});
```

### Option 2: Backend Service
Set up a backend endpoint to handle form submissions.

### Option 3: Formspree
Use Formspree for free form handling:
1. Visit https://formspree.io/
2. Create a form and get the endpoint
3. Update the form action in HTML

## Deployment

### Option 1: GitHub Pages (Free)
1. Create a GitHub repository named `portfolio`
2. Push your files to the repository
3. Go to Settings → Pages → Select main branch
4. Your site will be live at `https://yourusername.github.io/portfolio`

### Option 2: Custom Domain (GitHub Pages)
1. Follow the same steps as above
2. Add a `CNAME` file with your domain name
3. Update DNS settings with your domain registrar

### Option 3: Netlify (Free)
1. Go to https://netlify.com
2. Click "New site from Git"
3. Connect your GitHub repository
4. Deploy automatically on push

### Option 4: Vercel (Free)
1. Go to https://vercel.com
2. Import your GitHub repository
3. Deploy with one click

### Option 5: Web Hosting
Use traditional web hosting (GoDaddy, Bluehost, etc.) and upload files via FTP.

## SEO Optimization

Update the meta tags in `index.html`:

```html
<meta name="description" content="DevOps and SRE Engineer with 6+ years of experience">
<meta name="keywords" content="DevOps, SRE, Kubernetes, AWS, Terraform">
<meta name="author" content="Your Name">
<meta property="og:title" content="Pradumn Jha - DevOps Engineer">
<meta property="og:description" content="Your professional summary">
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Tips

1. **Optimize Images**: Compress images before adding them
2. **Lazy Loading**: Images load only when visible
3. **Caching**: Browsers cache static assets
4. **Minification**: Consider minifying CSS and JS for production

## Accessibility

- Semantic HTML structure
- Proper heading hierarchy
- Alt text for images (when added)
- Keyboard navigation support
- High contrast ratios for readability

## Browser Testing

Test your portfolio on:
- [BrowserStack](https://www.browserstack.com/) - Free trial
- [LambdaTest](https://www.lambdatest.com/) - Free trial
- Chrome DevTools - Built-in (F12)

## Analytics

Add Google Analytics:

```html
<!-- Add before closing </head> tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## Backup Resources

Example portfolios to reference:
- https://pradumnjha.com (referenced in your request)
- https://brittanychiang.com
- https://www.chromewebstore.google.com
- GitHub developer profiles

## Maintenance

Regular updates recommended:
- Update experience and projects
- Refresh technical skills
- Add new certifications
- Update achievement metrics
- Refresh design periodically

## Support & Further Help

For more information:
- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS-Tricks](https://css-tricks.com/)
- [Stack Overflow](https://stackoverflow.com/)

## License

Feel free to use this template for your personal portfolio.

---

**Last Updated**: January 2026
**Version**: 1.0
