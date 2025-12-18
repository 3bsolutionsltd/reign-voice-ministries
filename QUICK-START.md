# 🚀 Quick Start Guide

## View Your Website Right Now

### Option 1: Double-Click (Easiest)
1. Navigate to `c:\Users\DELL\churchwebsite`
2. Double-click `index.html`
3. Website opens in your default browser

### Option 2: Live Server in VS Code (Best for Editing)
1. Install "Live Server" extension in VS Code
2. Right-click `index.html`
3. Select "Open with Live Server"
4. Website opens at `http://localhost:5500`
5. Auto-refreshes when you save changes

### Option 3: Python Server
Open PowerShell in the project folder and run:
```powershell
cd c:\Users\DELL\churchwebsite
python -m http.server 8000
```
Then open: `http://localhost:8000`

## 📝 First Steps Customization

### 1. Update Church Information (5 minutes)

**index.html** - Search and replace:
- `info@soronkochurch.org` → Your actual email
- `Soronko Village` → Your full address
- `10:00 AM` → Your actual service time

### 2. Personalize Content (10 minutes)

**Edit these sections in index.html:**

**Hero Section** (Lines ~30-40):
```html
<h1 class="hero-title">Come Be Part of God's Work</h1>
<p class="hero-subtitle">Join us in building His kingdom in Soronko Village</p>
```
Change to match your church's voice and message.

**Building Project Story** (Lines ~75-85):
Update with your actual project details and current needs.

**Ministry Descriptions** (Lines ~150-250):
Customize each ministry description to reflect your actual programs.

### 3. Add Your First Photo (15 minutes)

1. Take or get a photo of your church building
2. Resize to 800x600 pixels (use https://squoosh.app)
3. Save as `church-building.jpg`
4. Put in `images` folder
5. In `index.html`, find:
```html
<div class="placeholder-image building">
```
6. Replace entire div with:
```html
<img src="images/church-building.jpg" alt="Soronko Church Building Progress">
```

### 4. Change Colors (5 minutes)

**styles.css** - Lines 5-10:
```css
--primary-color: #2c5f2d;      /* Change this to your preferred green */
--secondary-color: #d4a574;    /* Change this to your preferred gold/accent */
```

Use color picker: https://htmlcolorcodes.com/

## 🎨 Design Tips

### Colors that Work Well for Churches:
- **Blues**: Trust, peace → `#2c5f8d` (Ocean Blue)
- **Greens**: Growth, life → `#2c5f2d` (Forest Green) - Current
- **Purples**: Royalty → `#6b2c5f` (Royal Purple)
- **Golds**: Value, warmth → `#d4a574` (Warm Gold) - Current

### Font Alternatives:
In `index.html`, replace the Google Fonts link with:

**More Traditional:**
```html
<link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@300;400;700&family=Open+Sans:wght@300;400;600;700&display=swap" rel="stylesheet">
```
Then update CSS:
```css
--font-primary: 'Open Sans', sans-serif;
--font-display: 'Merriweather', serif;
```

**More Modern:**
```html
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&family=Montserrat:wght@600;700;800&display=swap" rel="stylesheet">
```
Then update CSS:
```css
--font-primary: 'Poppins', sans-serif;
--font-display: 'Montserrat', sans-serif;
```

## 📱 Test Checklist

Before sharing with others:

- [ ] View on your phone
- [ ] View on tablet (if available)
- [ ] Try the mobile menu (click hamburger icon)
- [ ] Scroll through entire page
- [ ] Click all navigation links
- [ ] Test contact form submission
- [ ] Check all text for typos
- [ ] Verify all information is accurate

## 🔧 Common Customizations

### Change Navigation Items

**index.html** - Lines ~20-25:
```html
<a href="#discover" class="nav-link">Discover</a>
<a href="#connect" class="nav-link">Connect</a>
<a href="#give" class="nav-link nav-link-highlight">Give</a>
```

Add new item:
```html
<a href="#events" class="nav-link">Events</a>
```

### Add Social Media Icons

In footer section:
```html
<div class="footer-col">
    <h4>Follow Us</h4>
    <div class="social-links">
        <a href="https://facebook.com/yourchurch">Facebook</a>
        <a href="https://instagram.com/yourchurch">Instagram</a>
        <a href="https://youtube.com/yourchurch">YouTube</a>
    </div>
</div>
```

### Adjust Section Order

You can rearrange sections by cutting and pasting entire section blocks:
- Building Project
- Discover
- Ministries
- Connect
- Give

Just move the entire `<section>` tags around.

## 🆘 Quick Fixes

### Problem: Colors look wrong
- Check your monitor brightness
- View on different devices
- Ask others for feedback

### Problem: Text too small/large
In `styles.css`, adjust:
```css
html {
    font-size: 16px; /* Change to 14px (smaller) or 18px (larger) */
}
```

### Problem: Sections too cramped/spacious
In `styles.css`, adjust spacing variables:
```css
--spacing-lg: 4rem; /* Increase for more space, decrease for less */
--spacing-xl: 6rem;
```

## 📚 Learn More

### HTML Basics:
- W3Schools: https://www.w3schools.com/html/
- MDN Web Docs: https://developer.mozilla.org/en-US/docs/Web/HTML

### CSS Styling:
- CSS Tricks: https://css-tricks.com/
- Flexbox Guide: https://css-tricks.com/snippets/css/a-guide-to-flexbox/

### JavaScript:
- JavaScript.info: https://javascript.info/
- FreeCodeCamp: https://www.freecodecamp.org/

## 💡 Content Ideas

### Add to Your Website Later:
1. **Events Calendar** - Upcoming church activities
2. **Blog/News** - Share updates and testimonials
3. **Photo Gallery** - Ministry and event photos
4. **Sermon Archive** - Past messages (audio/video)
5. **Online Giving Dashboard** - Track project progress
6. **Member Directory** - For registered members
7. **Prayer Wall** - Community prayer requests
8. **Resources** - Bible study materials
9. **Volunteer Signup** - For ministry involvement
10. **Impact Stories** - Testimonies and transformations

## 🎯 Next Steps

1. ✅ View website locally
2. ✅ Make basic customizations
3. ✅ Get feedback from church leadership
4. ✅ Add real photos
5. ✅ Test thoroughly
6. ✅ Choose hosting service (see DEPLOYMENT.md)
7. ✅ Deploy online
8. ✅ Set up forms and donations
9. ✅ Announce to congregation
10. ✅ Share on social media

## 📞 Need Help?

**Documentation Files:**
- `README.md` - Complete overview
- `DEPLOYMENT.md` - How to publish online
- `IMAGE-GUIDE.md` - Photo specifications
- `QUICK-START.md` - This file

**Online Resources:**
- Stack Overflow (for code questions)
- YouTube (for video tutorials)
- Fiverr (hire help $50-200)

---

## 🎉 You're Ready!

Your church website is built and ready to customize. Take it step by step, and don't be afraid to experiment. You can always undo changes.

**Remember**: The goal is to share God's work in Soronko with the world. Your website will help connect your church with supporters and partners globally.

**God bless your ministry! 🙏**

---

**Version**: 1.0  
**Last Updated**: December 2025  
**Created for**: Soronko Village Church, Eastern Uganda
