# Image Guidelines for Soronko Village Church Website

## 📁 Image Folder Structure

```
images/
├── hero/
│   └── church-hero.jpg           (1920x1080px) - Main hero background
├── building/
│   ├── progress-1.jpg            (800x600px) - Current building state
│   ├── progress-2.jpg            (800x600px) - Different angle
│   ├── foundation.jpg            (800x600px) - Early stages
│   └── ring-beam.jpg             (800x600px) - Ring beam stage
├── ministries/
│   ├── community-outreach.jpg    (600x400px) - Community service
│   ├── children-ministry.jpg     (600x400px) - Kids activities
│   ├── women-ministry.jpg        (600x400px) - Women's fellowship
│   └── men-ministry.jpg          (600x400px) - Men's group
├── church/
│   ├── sunday-service.jpg        (800x600px) - Worship service
│   ├── worship-team.jpg          (600x400px) - Worship leaders
│   ├── pastor.jpg                (400x400px) - Church pastor
│   └── congregation.jpg          (800x600px) - Full congregation
└── logo/
    ├── church-logo.png           (500x500px) - Main logo
    └── church-logo-white.png     (500x500px) - White version
```

## 📸 Photo Shooting Guidelines

### Building Project Photos
**What to capture:**
- Current construction stage (ring beam)
- Wide angle showing entire structure
- Close-ups of construction details
- Before and during photos side-by-side
- Workers/volunteers on site
- Foundation and completed portions

**Best practices:**
- Shoot during golden hour (early morning/late afternoon)
- Show scale by including people in shots
- Capture progress from consistent angles for comparison
- Take both landscape and portrait orientations

### Ministry Photos
**Community Outreach:**
- Food distribution events
- Medical outreach activities
- Community gatherings
- Helping vulnerable members
- Village interaction scenes

**Children's Ministry:**
- Kids learning Bible stories
- Singing and worship activities
- Arts and crafts
- Playing and fellowship
- Teacher-student interactions

**Women's Ministry:**
- Bible study groups
- Prayer circles
- Skills training sessions
- Fellowship meals
- Leadership meetings

**Men's Ministry:**
- Men's fellowship gatherings
- Service projects
- Bible study sessions
- Mentorship activities
- Community building work

### Sunday Service Photos
**Essential shots:**
- Full congregation (from back of church)
- Worship team leading praise
- Pastor preaching
- People worshiping (hands raised, praying)
- Communion/baptism ceremonies
- Children's church activities
- After-service fellowship

**Tips:**
- Get permission before photographing people
- Capture genuine moments (candid shots)
- Show diversity and engagement
- Avoid flash during service (use natural light)

## 🎨 Image Specifications

### File Formats
- **Photos**: JPG/JPEG (optimized for web)
- **Graphics/Icons**: PNG (for transparency)
- **Logo**: PNG or SVG (vector format preferred)

### Size Recommendations

| Image Type | Dimensions | File Size |
|------------|------------|-----------|
| Hero Background | 1920x1080px | < 500KB |
| Large Photos | 800x600px | < 300KB |
| Medium Photos | 600x400px | < 200KB |
| Small Photos | 400x400px | < 150KB |
| Thumbnails | 300x200px | < 100KB |
| Logo | 500x500px | < 100KB |

### Aspect Ratios
- **Hero**: 16:9 (landscape)
- **Building Photos**: 4:3 (landscape)
- **Ministry Cards**: 3:2 (landscape)
- **Portrait Photos**: 1:1 (square)

## 🖼️ Image Optimization Tools

### Online Tools (Free)
1. **TinyPNG** (https://tinypng.com/)
   - Reduces file size without losing quality
   - Batch processing available

2. **Squoosh** (https://squoosh.app/)
   - Google's image compression tool
   - Real-time quality preview

3. **Compressor.io** (https://compressor.io/)
   - Simple drag-and-drop interface
   - Supports multiple formats

### Desktop Software
1. **GIMP** (Free)
   - Full-featured photo editor
   - Export for web option

2. **Adobe Photoshop** (Paid)
   - Professional editing
   - Save for web feature

3. **IrfanView** (Free - Windows)
   - Batch conversion and resizing
   - Fast and lightweight

## 📝 How to Add Images to the Website

### Step 1: Prepare Your Images
1. Rename images descriptively (e.g., `children-ministry-worship.jpg`)
2. Resize to recommended dimensions
3. Optimize file size
4. Place in appropriate folder

### Step 2: Update HTML Code

**For Building Project Section:**

Find this in `index.html`:
```html
<div class="placeholder-image building">
    <span>Building Progress Photo</span>
</div>
```

Replace with:
```html
<img src="images/building/ring-beam.jpg" alt="Church Building Progress - Ring Beam Stage">
```

**For Ministry Cards:**

Find:
```html
<div class="placeholder-image community">
    <span>Community Outreach</span>
</div>
```

Replace with:
```html
<img src="images/ministries/community-outreach.jpg" alt="Community Outreach Ministry">
```

**For Hero Background:**

Add this to `styles.css` in the `.hero` section:
```css
.hero {
    background-image: url('../images/hero/church-hero.jpg');
    background-size: cover;
    background-position: center;
}
```

### Step 3: Add Alt Text
Always include descriptive alt text for accessibility:
```html
<img src="images/photo.jpg" alt="Descriptive text of what's in the image">
```

**Good examples:**
- "Children singing during Sunday worship service"
- "Pastor John delivering sermon"
- "Church building construction at ring beam stage"
- "Women's ministry Bible study group"

## 🎭 Creating Images if Photos Aren't Available Yet

### Temporary Solutions:

1. **Free Stock Photos**
   - Unsplash: https://unsplash.com/
   - Pexels: https://pexels.com/
   - Pixabay: https://pixabay.com/
   
   Search terms: "church", "worship", "community", "Uganda", "Africa", "construction"

2. **Design Custom Graphics**
   - Canva: https://canva.com/ (Free templates)
   - Create simple colored backgrounds with text overlays
   - Use icons and illustrations

3. **AI-Generated Placeholders**
   - Use colored backgrounds (already in CSS)
   - Add inspiring text quotes
   - Use symbolic imagery

## 📱 Social Media Image Sizes

For sharing the website on social media:

**Facebook:**
- Shared Link: 1200x630px
- Profile Image: 180x180px
- Cover Photo: 820x312px

**Instagram:**
- Feed Post: 1080x1080px (square)
- Story: 1080x1920px (vertical)

**Twitter:**
- Shared Link: 1200x628px
- Header: 1500x500px

Create an `images/social/` folder with these optimized versions.

## ✅ Image Quality Checklist

Before uploading any image, verify:
- [ ] Image is clear and well-lit
- [ ] Proper dimensions and aspect ratio
- [ ] File size optimized for web
- [ ] Appropriate file format (JPG/PNG)
- [ ] Descriptive filename (no spaces, use hyphens)
- [ ] People in photos have given permission
- [ ] Image represents church values positively
- [ ] Colors match website color scheme
- [ ] Text is readable if overlaid

## 🎨 Photo Editing Tips

### Basic Edits for Church Photos:
1. **Brightness/Contrast**: Ensure faces are visible
2. **Crop**: Remove distracting elements
3. **Saturation**: Slightly increase for vibrancy (don't overdo)
4. **Straighten**: Level horizons in building photos
5. **Remove**: Blur or remove identifying info if needed

### Consistent Look:
- Apply similar filters to all ministry photos
- Keep color temperature consistent
- Maintain similar brightness levels
- Use same aspect ratios within sections

## 🔒 Copyright and Permissions

**Remember:**
1. Get written permission to photograph people
2. Obtain parental consent for children's photos
3. Don't use copyrighted images without permission
4. Credit photographers if required
5. Respect people's privacy

**Model Release Template:**
Create a simple form stating:
- Photo will be used on church website
- Name and signature of person photographed
- Parent/guardian signature for minors
- Date

## 📞 Professional Photography

If budget allows, consider hiring a local photographer for:
- Professional church directory
- High-quality building project documentation
- Ministry event coverage
- Promotional materials

**Cost**: Usually $100-500 USD depending on hours and deliverables

## 🎬 Video Content

Consider adding video in the future:
- Time-lapse of building construction
- Pastor welcome message
- Ministry spotlights
- Worship service clips
- Testimonials

**Hosting options:**
- YouTube (Free, unlimited)
- Vimeo (Professional, paid plans)
- Embed directly on website

---

**Questions?** Refer to the main README.md or consult with a web designer.

**May your images tell the powerful story of God's work in Soronko! 📸**
