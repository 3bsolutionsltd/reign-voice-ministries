# Soronko Village Church Website

A beautiful, modern website for Soronko Village Church in Eastern Uganda, designed to showcase the church's ministries, building project, and provide a platform for global partnership.

## 🎯 Project Overview

This website was created to help Soronko Village Church:
- Share their 12-year building project journey with the world
- Connect with potential partners and supporters globally
- Showcase their various ministries (Community Outreach, Children, Women, Men)
- Provide an easy way for people to give and support the church
- Tell their story and God's work in their community

## 📁 Project Structure

```
churchwebsite/
├── index.html          # Main HTML structure
├── styles.css          # All styling and responsive design
├── script.js           # Interactive features and animations
└── README.md           # This file
```

## 🎨 Design Features

### Navigation
- **Discover**: Learn about the church's story, mission, and Sunday services
- **Connect**: Get in touch, submit prayer requests, and stay updated
- **Give**: Support the building project and various ministries

### Key Sections

1. **Hero Section**
   - Compelling call-to-action
   - Beautiful gradient background
   - Clear buttons to engage visitors

2. **Building Project Highlight**
   - Prominently features the 12-year building project
   - Current stage: Ring beam
   - Visual stats and project story
   - Direct call-to-action for partnership

3. **Discover Section**
   - Church story and mission
   - Sunday service information
   - Core values and beliefs

4. **Ministries Section**
   - Community Outreach (Featured)
   - Children's Ministry
   - Women's Ministry
   - Men's Ministry
   - Each with detailed descriptions and activities

5. **Connect Section**
   - Visit information
   - Contact details
   - Newsletter signup form
   - Prayer request submission

6. **Give Section**
   - Building Project Fund (Primary focus)
   - General Ministry Fund
   - Sponsor a Ministry options
   - Multiple giving methods

## 🎨 Color Scheme

The website uses a nature-inspired, warm color palette:

- **Primary Green**: `#2c5f2d` - Represents growth and life
- **Secondary Gold**: `#d4a574` - Represents value and blessing
- **Accent Cream**: `#faf8f5` - Warm and welcoming background

## 📱 Responsive Design

The website is fully responsive and works beautifully on:
- Desktop computers (1200px+)
- Tablets (768px - 1200px)
- Mobile phones (< 768px)

## ✨ Interactive Features

- Smooth scroll navigation
- Mobile-friendly hamburger menu
- Fade-in animations on scroll
- Parallax hero effect
- Back-to-top button
- Form validation
- Hover effects on all interactive elements

## 🚀 Getting Started

### Option 1: Open Directly
1. Simply double-click `index.html` to open in your browser

### Option 2: Use Live Server (Recommended)
1. Install the "Live Server" extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"
4. The site will open at `http://localhost:5500`

### Option 3: Python Server
```bash
# Navigate to the project folder
cd c:\Users\DELL\churchwebsite

# Python 3
python -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## 🔧 Customization Guide

### 1. Replace Placeholder Images

The current design uses colored placeholders. Replace them with actual photos:

In `index.html`, find sections like:
```html
<div class="placeholder-image building">
    <span>Building Progress Photo</span>
</div>
```

Replace with:
```html
<img src="images/building-progress.jpg" alt="Building Progress">
```

**Recommended image sizes:**
- Hero background: 1920x1080px
- Building project photos: 800x600px
- Ministry photos: 600x400px

### 2. Update Church Information

**Contact Details** (in Connect and Footer sections):
- Replace `info@soronkochurch.org` with actual email
- Add phone number if available
- Update address details

**Service Times**:
- Update Sunday service time (currently set to 10:00 AM)
- Add any other service times

### 3. Customize Colors

In `styles.css`, update the CSS variables:
```css
:root {
    --primary-color: #2c5f2d;      /* Change to your preference */
    --secondary-color: #d4a574;    /* Change to your preference */
}
```

### 4. Add Social Media Links

In the footer section of `index.html`, add:
```html
<div class="social-links">
    <a href="https://facebook.com/yourchurch">Facebook</a>
    <a href="https://instagram.com/yourchurch">Instagram</a>
    <a href="https://youtube.com/yourchurch">YouTube</a>
</div>
```

### 5. Set Up Form Submission

The contact form currently shows an alert. To make it functional:

**Option A: EmailJS (Free)**
1. Sign up at [emailjs.com](https://www.emailjs.com/)
2. Add the EmailJS script to `index.html` before `</body>`:
```html
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
```
3. Update `script.js` form handler with EmailJS configuration

**Option B: Formspree (Free)**
1. Sign up at [formspree.io](https://formspree.io/)
2. Update the form action:
```html
<form class="newsletter-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### 6. Add Google Analytics

Before `</head>` in `index.html`:
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

## 💳 Setting Up Online Donations

### Recommended Options:

1. **PayPal Donate Button**
   - Free for nonprofits
   - Easy to set up
   - International support

2. **Stripe**
   - Professional payment processing
   - Recurring donations support
   - 2.9% + $0.30 per transaction

3. **Flutterwave** (African-friendly)
   - Designed for African businesses
   - Multiple payment methods
   - Mobile money integration

4. **Give WordPress Plugin**
   - If you move to WordPress later
   - Comprehensive donation management

## 📸 Creating Images

If you need to create placeholder images before having actual photos:

**Free Design Tools:**
- [Canva](https://www.canva.com/) - Easy drag-and-drop design
- [Figma](https://www.figma.com/) - Professional design tool
- [Unsplash](https://unsplash.com/) - Free high-quality photos

**Recommended Photos to Take:**
- Current building progress (multiple angles)
- Sunday service worship scenes
- Children's ministry activities
- Community outreach programs
- Church leaders and pastors
- Women's and Men's ministry gatherings

## 🌐 Deployment Options

### Free Hosting Options:

1. **GitHub Pages** (Recommended)
   ```bash
   # Create a GitHub account
   # Create a repository named: yourusername.github.io
   # Upload all files
   # Access at: https://yourusername.github.io
   ```

2. **Netlify**
   - Drag and drop deployment
   - Custom domain support
   - Free SSL certificate

3. **Vercel**
   - Similar to Netlify
   - Fast deployment
   - Great performance

### Steps for GitHub Pages:
1. Create a free account at [github.com](https://github.com)
2. Create a new repository
3. Upload your files (index.html, styles.css, script.js)
4. Go to Settings > Pages
5. Select the main branch
6. Your site will be live at `https://yourusername.github.io/repository-name`

## 🎓 SEO Optimization

Add these meta tags to `<head>` section in `index.html`:

```html
<!-- Primary Meta Tags -->
<meta name="title" content="Soronko Village Church - Eastern Uganda">
<meta name="description" content="Join us in building God's kingdom in Soronko Village. Support our 12-year building project and discover our ministries.">
<meta name="keywords" content="Soronko Church, Eastern Uganda Church, Church Building Project, Uganda Ministry">

<!-- Open Graph / Facebook -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://yourwebsite.com/">
<meta property="og:title" content="Soronko Village Church - Eastern Uganda">
<meta property="og:description" content="Join us in building God's kingdom in Soronko Village.">
<meta property="og:image" content="https://yourwebsite.com/images/og-image.jpg">

<!-- Twitter -->
<meta property="twitter:card" content="summary_large_image">
<meta property="twitter:url" content="https://yourwebsite.com/">
<meta property="twitter:title" content="Soronko Village Church - Eastern Uganda">
<meta property="twitter:description" content="Join us in building God's kingdom in Soronko Village.">
<meta property="twitter:image" content="https://yourwebsite.com/images/twitter-image.jpg">
```

## 📱 Future Enhancements

Consider adding:
- [ ] Blog/News section for church updates
- [ ] Event calendar
- [ ] Sermon audio/video archive
- [ ] Online Bible study resources
- [ ] Member login area
- [ ] Photo gallery
- [ ] Testimonials section
- [ ] Live streaming capability
- [ ] Multi-language support (English/Local language)

## 🐛 Troubleshooting

**Problem**: Fonts not loading
- **Solution**: Check internet connection (fonts load from Google Fonts)

**Problem**: Images not showing
- **Solution**: Make sure image paths are correct and images are in the right folder

**Problem**: Mobile menu not working
- **Solution**: Ensure `script.js` is properly linked in `index.html`

**Problem**: Smooth scrolling not working
- **Solution**: Check that all section IDs match the href attributes in navigation links

## 📞 Support & Questions

If you need help customizing this website:
1. Check this README first
2. Review the code comments in each file
3. Search for tutorials on HTML/CSS/JavaScript basics
4. Consider hiring a web developer for advanced customizations

## 📄 License

This website template is created for Soronko Village Church. Feel free to customize it for your needs.

## 🙏 Acknowledgments

- Design inspiration from [BeLoved Church](https://www.belovedchurch.ca/)
- Built with modern web standards
- Created with love for God's glory

---

**Last Updated**: December 2025  
**Created by**: Website Developer for Soronko Village Church  
**Contact**: For website support, reach out to the development team

## 🚀 Quick Start Checklist

- [ ] Replace placeholder text with actual church information
- [ ] Add real photos and images
- [ ] Update contact information
- [ ] Set up form submission service
- [ ] Add social media links
- [ ] Configure donation payment system
- [ ] Add Google Analytics
- [ ] Test on multiple devices
- [ ] Deploy to web hosting
- [ ] Set up custom domain (if available)
- [ ] Share with church leadership for feedback
- [ ] Launch and share with the community!

---

**God bless the work of your hands! 🙏**
