# DunamisLAN Event Website

A static website for hosting LAN party event information, registration, and community links. Built to be hosted on GitHub Pages with a custom subdomain (lan.dunamisnexus.net).

## 🚀 Quick Start

1. **Clone/Create your repository** (if you haven't already)
2. **Add the website files** to your repository
3. **Create the folder structure** (see below)
4. **Add your images**
5. **Customize the content**
6. **Enable GitHub Pages**
7. **Configure your custom domain**

## 📁 Folder Structure

Create this structure in your repository:

```
your-repo/
├── index.html          (main page - already created)
├── styles.css          (styling - already created)
├── script.js           (JavaScript - already created)
├── README.md          (this file)
└── images/
    ├── logo.png       (YOUR LOGO - add this)
    ├── hero-bg.jpg    (HERO BACKGROUND - optional)
    └── gallery/
        ├── event1.jpg (PAST EVENT PHOTOS)
        ├── event2.jpg
        ├── event3.jpg
        └── ... (add as many as you want)
```

## 🖼️ Adding Images

### 1. Logo
- **Location:** `images/logo.png`
- **Purpose:** Appears in the navigation bar
- **Recommended size:** 200x200px (transparent background PNG)
- **Format:** PNG with transparency

### 2. Hero Background (Optional)
- **Location:** `images/hero-bg.jpg`
- **Purpose:** Large background image for the hero section
- **Recommended size:** 1920x1080px or larger
- **Format:** JPG or PNG
- **Note:** If you don't add this, the gradient background will still look great!

### 3. Gallery/Carousel Images
- **Location:** `images/gallery/`
- **Files:** `event1.jpg`, `event2.jpg`, `event3.jpg`, etc.
- **Purpose:** Slideshow of past LAN party events
- **Recommended size:** 1200x800px (landscape orientation)
- **Format:** JPG or PNG

**To add more gallery images:**
1. Add image files to `images/gallery/`
2. Open `index.html`
3. Find the carousel section (around line 90)
4. Copy/paste a carousel slide and update the image name:

```html
<div class="carousel-slide">
    <img src="images/gallery/event4.jpg" alt="Past LAN Event 4">
    <div class="carousel-caption">DunamisLAN Event</div>
</div>
```

## ✏️ Customization Guide

### Essential Updates

#### 1. Add Your Tagline
**File:** `index.html` (line ~45)
```html
<p class="tagline">Your awesome tagline goes here!</p>
```

#### 2. Update Discord Link
**File:** `index.html` (lines ~23 and ~302)
```html
<!-- In navigation -->
<li><a href="https://discord.gg/YOUR_DISCORD_INVITE" target="_blank" class="discord-link">Discord</a></li>

<!-- In links section -->
<a href="https://discord.gg/YOUR_DISCORD_INVITE" target="_blank" class="link-card">
```

#### 3. Update PayPal Link
**File:** `index.html` (line ~157)
```html
<a href="https://paypal.me/YOUR_PAYPAL" target="_blank" class="btn btn-paypal">
```

#### 4. Configure Registration

**Option A: Embedded Google Form**
1. Create your Google Form
2. Click "Send" → "Embed HTML"
3. Copy the iframe code
4. In `index.html` (around line ~144), uncomment and paste:

```html
<div class="registration-form">
    <iframe src="YOUR_GOOGLE_FORM_EMBED_URL" width="100%" height="800" frameborder="0">Loading…</iframe>
</div>
```

**Option B: External Registration Link**
- In `index.html` (around line ~151), update the href:

```html
<a href="https://YOUR_REGISTRATION_LINK" target="_blank" class="btn btn-primary btn-large">
    Register via LANReg
</a>
```

#### 5. Update Event Information
**File:** `index.html` (lines ~129-133)
```html
<p class="event-date">📅 Date: Saturday, March 15, 2025</p>
<p class="event-location">📍 Location: 123 Gaming St, City, State</p>
<p class="event-cost">💵 Cost: $25 per person</p>
<p class="event-capacity">👥 Capacity: 50 players</p>
```

#### 6. Update Schedule
**File:** `index.html` (starting around line ~181)
- Modify times and activities to match your event schedule

#### 7. Customize Colors (Optional)
**File:** `styles.css` (lines 5-18)
```css
:root {
    --primary-color: #4a90e2;      /* Main blue */
    --secondary-color: #7b68ee;     /* Purple accent */
    --accent-color: #00d4ff;        /* Cyan highlight */
    /* Modify these to match your brand! */
}
```

## 🌐 GitHub Pages Setup

### Step 1: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings**
3. Scroll down to **Pages** (in the left sidebar)
4. Under **Source**, select:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
5. Click **Save**

Your site will be published at: `https://yourusername.github.io/your-repo-name/`

### Step 2: Configure Custom Domain (lan.dunamisnexus.net)

#### A. In GitHub Repository:
1. In **Settings** → **Pages**
2. Under **Custom domain**, enter: `lan.dunamisnexus.net`
3. Click **Save**
4. Check **Enforce HTTPS** (after DNS propagates)

#### B. In Your DNS Provider (where dunamisnexus.net is hosted):
Add a **CNAME record**:
- **Type:** CNAME
- **Host/Name:** `lan`
- **Value/Target:** `yourusername.github.io`
- **TTL:** 3600 (or default)

**Example:**
```
lan.dunamisnexus.net → CNAME → yourusername.github.io
```

**Note:** DNS changes can take 24-48 hours to fully propagate.

### Step 3: Verify Setup
After DNS propagates:
1. Visit `https://lan.dunamisnexus.net`
2. Your site should load with HTTPS!

## 📝 Content Guidelines

### About Section
Update the text to describe your specific LAN events, community, and what makes your events special.

### FAQ Section
Add/modify questions based on what your attendees commonly ask:
- What to bring
- Food arrangements
- Age requirements
- Spectator policy
- etc.

### Rules Section
Customize rules based on your venue requirements and community standards.

### Links Section
The links are already configured for Dunamis Nexus properties. Verify they're all correct:
- Main website
- Discord
- Forum
- Mastodon
- Ko-fi
- Merch store

## 🎨 Design Features

- ✅ **Fully Responsive** - Works on desktop, tablet, and mobile
- ✅ **Dark Theme** - Matches Dunamis Nexus branding
- ✅ **Image Carousel** - Auto-advancing slideshow with manual controls
- ✅ **Smooth Animations** - Fade-in effects and smooth scrolling
- ✅ **Mobile Menu** - Hamburger menu for small screens
- ✅ **Touch Gestures** - Swipe to navigate carousel on mobile

## 🔧 Troubleshooting

### Images not showing?
- Check file paths are correct (case-sensitive!)
- Ensure images are in the correct folders
- Check image file formats (use JPG or PNG)

### Custom domain not working?
- Wait 24-48 hours for DNS propagation
- Verify CNAME record is correct
- Check GitHub Pages settings
- Clear your browser cache

### Carousel not working?
- Make sure you have at least 2 images in the gallery
- Check browser console for JavaScript errors
- Ensure `script.js` is linked correctly in HTML

### Mobile menu not toggling?
- Check that `script.js` is loaded
- Verify JavaScript console for errors
- Try a hard refresh (Ctrl+F5)

## 📱 Testing Checklist

Before going live, test:
- [ ] All internal links (navigation, buttons)
- [ ] All external links (Discord, main site, etc.)
- [ ] Carousel navigation (arrows, dots, keyboard, swipe)
- [ ] Mobile menu (hamburger icon)
- [ ] Registration form/link
- [ ] Payment buttons (Ko-fi, PayPal)
- [ ] Responsive design on different screen sizes
- [ ] All images load correctly
- [ ] Custom domain works

## 🚀 Going Live Checklist

- [ ] Add all your images
- [ ] Update tagline
- [ ] Update event information (date, location, cost, capacity)
- [ ] Configure registration (Google Form or external link)
- [ ] Update Discord invite link
- [ ] Update PayPal link
- [ ] Customize schedule
- [ ] Review and update FAQ
- [ ] Review and update rules
- [ ] Test all links and features
- [ ] Enable GitHub Pages
- [ ] Configure custom domain DNS
- [ ] Wait for DNS propagation
- [ ] Verify HTTPS is working
- [ ] Test on multiple devices

## 💡 Future Enhancements

Consider adding:
- Past winners/highlights section
- Sponsor logos section
- Live countdown timer to next event
- Newsletter signup
- Social media feed integration
- Interactive map for venue location

## 📞 Support

If you need help:
1. Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
2. Ask in the Dunamis Nexus Discord or forum
3. Search for solutions on Stack Overflow

## 📄 License

Feel free to modify and use this template for your events!

---

Built with ❤️ for the Dunamis Nexus community
Building Community Through Faith and Gaming
