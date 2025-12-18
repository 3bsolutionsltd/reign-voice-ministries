# 🚀 Deployment Guide - Soronko Village Church Website

This guide will help you publish your church website online so people around the world can access it.

## 📋 Pre-Deployment Checklist

Before going live, ensure:
- [ ] All church information is accurate (address, email, phone)
- [ ] You've replaced placeholder images with real photos
- [ ] Contact form is connected to email service
- [ ] All links work correctly
- [ ] Website tested on mobile devices
- [ ] Someone has proofread all content
- [ ] Donation/giving system is set up (if applicable)
- [ ] Google Analytics is configured (optional)

## 🌐 Deployment Options

### Option 1: GitHub Pages (FREE) ⭐ RECOMMENDED

**Best for**: Simple, free hosting with custom domain support

**Steps:**

1. **Create GitHub Account**
   - Go to https://github.com
   - Click "Sign Up"
   - Choose a username (e.g., "soronkochurch")
   - Verify your email

2. **Create Repository**
   - Click the "+" icon in top right
   - Select "New repository"
   - Name it: `soronkochurch.github.io` (or your preferred name)
   - Make it Public
   - Click "Create repository"

3. **Upload Files**
   
   **Method A: Web Upload (Easiest)**
   - Click "uploading an existing file"
   - Drag and drop all your files:
     - index.html
     - styles.css
     - script.js
     - README.md
     - images folder (with all contents)
   - Add commit message: "Initial website upload"
   - Click "Commit changes"

   **Method B: GitHub Desktop (Better for updates)**
   - Download GitHub Desktop: https://desktop.github.com/
   - Install and sign in
   - Clone your repository
   - Copy your files into the cloned folder
   - Commit and push changes

4. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to "Pages" section
   - Under "Source", select "main" branch
   - Click "Save"
   - Wait 2-3 minutes

5. **Access Your Site**
   - Your site will be live at: `https://yourusername.github.io/repository-name`
   - Example: `https://soronkochurch.github.io`

**Advantages:**
- ✅ Completely free
- ✅ Fast and reliable
- ✅ Free SSL certificate (HTTPS)
- ✅ Easy updates via GitHub
- ✅ Custom domain support

**Disadvantages:**
- ❌ Requires GitHub account
- ❌ Repository must be public (or paid plan)

---

### Option 2: Netlify (FREE)

**Best for**: Simple drag-and-drop deployment with excellent features

**Steps:**

1. **Create Account**
   - Go to https://www.netlify.com
   - Sign up with email or GitHub

2. **Deploy Site**
   - Click "Add new site" → "Deploy manually"
   - Create a ZIP file of your website folder
   - Drag and drop the ZIP file
   - Wait for deployment (usually 30 seconds)

3. **Custom Domain (Optional)**
   - Go to "Domain settings"
   - Add your custom domain
   - Follow DNS configuration instructions

4. **Access Your Site**
   - You'll get a URL like: `random-name-123.netlify.app`
   - You can change "random-name-123" to something better

**Advantages:**
- ✅ Super easy deployment
- ✅ Automatic SSL
- ✅ Form handling built-in
- ✅ Continuous deployment
- ✅ Good free tier

**Disadvantages:**
- ❌ Random subdomain (unless custom domain)

---

### Option 3: Vercel (FREE)

**Best for**: Fast performance and good for future scaling

**Steps:**

1. **Create Account**
   - Go to https://vercel.com
   - Sign up with GitHub, GitLab, or email

2. **Deploy**
   - Click "Add New Project"
   - Import your GitHub repository OR
   - Drag and drop your project folder

3. **Configure**
   - Vercel auto-detects settings
   - Click "Deploy"
   - Wait for deployment

4. **Access Site**
   - Get URL like: `project-name.vercel.app`

**Advantages:**
- ✅ Extremely fast hosting
- ✅ Great performance
- ✅ Easy to use
- ✅ Automatic deployments

**Disadvantages:**
- ❌ Slightly complex for beginners

---

### Option 4: InfinityFree (FREE)

**Best for**: Traditional web hosting experience

**Steps:**

1. **Sign Up**
   - Go to https://infinityfree.net
   - Create free account

2. **Create Account**
   - Choose a subdomain or use custom domain
   - Set up hosting account

3. **Upload Files**
   - Access File Manager or use FTP
   - Upload all files to `htdocs` folder
   - Ensure `index.html` is in root

4. **Access Site**
   - Your site will be at: `yoursite.infinityfreeapp.com`

**Advantages:**
- ✅ Traditional hosting
- ✅ FTP access
- ✅ PHP/MySQL support (for future)
- ✅ File manager

**Disadvantages:**
- ❌ Ads on free plan
- ❌ Slower than modern hosts
- ❌ Daily resource limits

---

## 🌍 Custom Domain Setup

If you want a custom domain like `soronkochurch.org`:

### 1. Purchase Domain

**Budget-Friendly Registrars:**
- **Namecheap**: ~$10-15/year (.org, .com)
- **Google Domains**: ~$12/year
- **Porkbun**: ~$8-10/year
- **Cloudflare**: ~$8-10/year (at cost pricing)

**African Registrars:**
- **Afriregister**: African-focused
- **ZACR**: South African domains

### 2. Connect Domain to Hosting

**For GitHub Pages:**
```
1. In your repository, create a file named "CNAME"
2. Add your domain: soronkochurch.org
3. In your domain registrar, add DNS records:

   Type: A
   Name: @
   Value: 185.199.108.153
   
   Type: A
   Name: @
   Value: 185.199.109.153
   
   Type: A
   Name: @
   Value: 185.199.110.153
   
   Type: A
   Name: @
   Value: 185.199.111.153
   
   Type: CNAME
   Name: www
   Value: yourusername.github.io
```

**For Netlify:**
```
1. In Netlify dashboard, go to Domain Settings
2. Click "Add custom domain"
3. Enter your domain
4. Follow DNS instructions provided
```

**DNS Propagation:**
- Changes take 24-48 hours to propagate globally
- Use https://dnschecker.org to track progress

---

## 📧 Setting Up Contact Form

Your contact form needs a backend service to send emails.

### Option 1: Formspree (FREE - Recommended)

**Setup:**
1. Go to https://formspree.io
2. Sign up for free account
3. Create new form
4. Get your form endpoint

**Update HTML:**
```html
<form class="newsletter-form" 
      action="https://formspree.io/f/YOUR_FORM_ID" 
      method="POST">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" placeholder="Message"></textarea>
    <button type="submit">Send</button>
</form>
```

**Free Plan Includes:**
- 50 submissions/month
- Email notifications
- Spam filtering

### Option 2: EmailJS (FREE)

**Setup:**
1. Sign up at https://www.emailjs.com
2. Add email service (Gmail, Outlook, etc.)
3. Create email template
4. Get Service ID, Template ID, and Public Key

**Update script.js:**
```javascript
// Add EmailJS SDK before your script.js
// <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>

emailjs.init("YOUR_PUBLIC_KEY");

newsletterForm.addEventListener('submit', (e) => {
    e.preventDefault();
    
    emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', e.target)
        .then(() => {
            alert('Thank you! We will be in touch soon.');
            newsletterForm.reset();
        }, (error) => {
            alert('Oops! Something went wrong. Please try again.');
        });
});
```

**Free Plan:**
- 200 emails/month
- All features included

### Option 3: Netlify Forms (FREE on Netlify)

If hosting on Netlify:

```html
<form class="newsletter-form" 
      name="contact" 
      method="POST" 
      data-netlify="true">
    <input type="hidden" name="form-name" value="contact">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" placeholder="Message"></textarea>
    <button type="submit">Send</button>
</form>
```

**Free Plan:**
- 100 submissions/month
- Built-in spam filtering
- Email notifications

---

## 💳 Setting Up Donations

### Option 1: PayPal Donate Button (FREE)

**Steps:**
1. Create PayPal Business account
2. Go to PayPal Buttons
3. Create Donate button
4. Customize button
5. Get HTML code
6. Paste into your Give section

**Code Example:**
```html
<form action="https://www.paypal.com/donate" method="post" target="_blank">
    <input type="hidden" name="business" value="YOUR_PAYPAL_EMAIL">
    <input type="hidden" name="item_name" value="Church Building Project">
    <input type="submit" value="Donate via PayPal" class="btn btn-primary">
</form>
```

### Option 2: Stripe Payment Links (2.9% + 30¢)

**Steps:**
1. Sign up at https://stripe.com
2. Create Payment Link
3. Set amount or allow custom
4. Add description
5. Get shareable link

**Add to HTML:**
```html
<a href="YOUR_STRIPE_PAYMENT_LINK" class="btn btn-primary">
    Give to Building Project
</a>
```

### Option 3: Flutterwave (African-friendly)

**Best for Uganda/Africa:**
1. Sign up at https://flutterwave.com
2. Create payment link or button
3. Supports mobile money
4. Multiple African payment methods

**Fees**: ~3.8% per transaction

### Option 4: Mobile Money (Uganda)

**MTN Mobile Money:**
```
Business Name: Soronko Village Church
Account Number: XXXX-XXXX
```

**Airtel Money:**
```
Business Name: Soronko Village Church
Number: XXXX-XXXX
```

Add instructions in the Give section for local giving.

---

## 📊 Analytics Setup

### Google Analytics (FREE)

**Setup:**
1. Go to https://analytics.google.com
2. Create account
3. Add property for website
4. Get Measurement ID (G-XXXXXXXXXX)

**Add to index.html before `</head>`:**
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

**Track:**
- Page views
- User location
- Time on site
- Popular pages
- Device types

---

## 🔧 Post-Deployment Tasks

### 1. Test Everything
- [ ] Open site in different browsers (Chrome, Firefox, Safari, Edge)
- [ ] Test on mobile phone
- [ ] Test on tablet
- [ ] Click every link
- [ ] Submit contact form
- [ ] Try donation buttons
- [ ] Check all images load

### 2. Submit to Search Engines

**Google:**
```
1. Go to https://search.google.com/search-console
2. Add property (your website URL)
3. Verify ownership
4. Submit sitemap (if you create one)
```

**Bing:**
```
1. Go to https://www.bing.com/webmasters
2. Add site
3. Verify ownership
```

### 3. Social Media Setup

**Create Accounts:**
- Facebook Page: facebook.com/pages/create
- Instagram: instagram.com
- YouTube Channel: youtube.com

**Share Website:**
- Post announcement
- Add website to bio/about
- Share building project updates
- Post regularly about ministries

### 4. Create Business Listings

**Google My Business:**
- https://business.google.com
- Add church address
- Add website
- Upload photos
- Helps local SEO

### 5. Monitor Performance

**Tools:**
- Google Analytics: Track visitors
- Google Search Console: Monitor search presence
- PageSpeed Insights: Check site speed
- Mobile-Friendly Test: Ensure mobile compatibility

---

## 🆘 Troubleshooting

### Issue: Website not loading
**Solutions:**
- Wait 24-48 hours for DNS propagation
- Clear browser cache (Ctrl+Shift+Delete)
- Check if files uploaded correctly
- Verify hosting service is active

### Issue: Images not showing
**Solutions:**
- Check image file paths are correct
- Ensure images uploaded to correct folder
- Verify image file names match HTML
- Check file extensions (.jpg vs .jpeg)

### Issue: Contact form not working
**Solutions:**
- Verify form service configuration
- Check email service API keys
- Test with spam filter disabled
- Ensure JavaScript is enabled

### Issue: Site looks broken on mobile
**Solutions:**
- Test responsive design
- Check viewport meta tag in HTML
- Verify CSS media queries
- Test on actual devices, not just browser tools

---

## 💰 Cost Summary

**Completely Free Option:**
- Hosting: GitHub Pages (FREE)
- Form: Formspree (FREE 50/month)
- Domain: Use GitHub subdomain (FREE)
- **Total: $0/year**

**Professional Option:**
- Hosting: Netlify/Vercel (FREE)
- Domain: Namecheap ($10-15/year)
- Form: EmailJS (FREE 200/month)
- Email: Google Workspace ($6/month)
- **Total: ~$82/year**

**With Donations:**
- PayPal: Free setup, 2.9% + 30¢ per transaction
- Stripe: Free setup, 2.9% + 30¢ per transaction
- Flutterwave: Free setup, ~3.8% per transaction

---

## 📞 Getting Help

**Technical Issues:**
1. Check this guide first
2. Search error messages on Google
3. Ask on Stack Overflow
4. Contact hosting support

**Web Design Help:**
- Hire freelancer on Fiverr ($50-200)
- Local web developer
- Tech-savvy church member

**Content Help:**
- Church communications team
- Professional copywriter
- AI writing assistants (ChatGPT, Claude)

---

## 🎉 Launch Announcement

When ready to announce:

**Email Template:**
```
Subject: 🎉 Our Church Website is Live!

Dear [Church Family / Partners],

We're excited to announce that Soronko Village Church now has a website!

Visit us at: [YOUR-WEBSITE-URL]

Through this website, you can:
✓ Learn about our 12-year building project
✓ Discover our ministries
✓ Partner with us financially
✓ Stay connected with updates
✓ Submit prayer requests

Please share with friends and family who want to support our mission.

God bless,
[Church Leadership]
```

**Social Media Post:**
```
🎉 BIG NEWS! 🎉

Soronko Village Church is now online! 

Visit our new website to:
🏗️ See our building project progress
🙏 Learn about our ministries
❤️ Partner with us
📧 Stay connected

[YOUR-WEBSITE-URL]

Share with someone who needs to see God's work in Eastern Uganda!

#SoronkoChurch #EasternUganda #ChurchBuilding #Faith
```

---

**Congratulations on launching your church website! May it bring glory to God and connect your church with supporters worldwide! 🙏🌍**
