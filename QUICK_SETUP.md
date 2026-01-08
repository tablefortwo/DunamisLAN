# 🚀 Quick Setup Guide for DunamisLAN

## Immediate Next Steps (in order):

### 1. Upload Files to GitHub Repository
Upload these files to your GitHub repository:
- `index.html`
- `styles.css`
- `script.js`
- `CNAME`
- `.gitignore`
- `README.md`

### 2. Create Image Folders
In your repository, create this folder structure:
```
images/
├── logo.png (add your logo here)
├── hero-bg.jpg (optional background image)
└── gallery/
    ├── event1.jpg
    ├── event2.jpg
    └── event3.jpg
```

### 3. Add Placeholder Images (Temporary)
Until you have real images, you can:
- **Option A:** Use placeholder images from https://placehold.co/
  - Logo: https://placehold.co/200x200/4a90e2/white?text=DunamisLAN
  - Gallery: https://placehold.co/1200x800/1a1a1a/4a90e2?text=Event+Photo
- **Option B:** Skip adding hero-bg.jpg (the gradient will work fine)
- **Option C:** Use screenshots from your existing events

### 4. Critical Content Updates

Open `index.html` and update these RIGHT NOW:

**Line ~45 - Add Your Tagline:**
```html
<p class="tagline">Connecting Gamers Through Faith and Competition</p>
```

**Line ~23 - Discord Invite:**
```html
<li><a href="https://discord.gg/YOUR_ACTUAL_INVITE" target="_blank" class="discord-link">Discord</a></li>
```

**Lines ~129-133 - Next Event Info:**
```html
<p class="event-date">📅 Date: TBA - Coming Soon!</p>
<p class="event-location">📍 Location: Will be announced</p>
<p class="event-cost">💵 Cost: TBA</p>
<p class="event-capacity">👥 Capacity: TBA</p>
```

**Line ~151 - Registration Link:**
```html
<a href="#" onclick="alert('Registration opens soon!'); return false;" class="btn btn-primary btn-large">
    Registration Opening Soon
</a>
```

**Line ~157 - PayPal Link:**
```html
<a href="https://paypal.me/YOUR_PAYPAL_USERNAME" target="_blank" class="btn btn-paypal">
```

### 5. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Click **Pages** in left sidebar
4. Under **Source**:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 2-5 minutes
7. Your site will be live at: `https://yourusername.github.io/repo-name/`

### 6. Test the Site

Visit your GitHub Pages URL and check:
- ✅ Site loads correctly
- ✅ Navigation works (click links)
- ✅ Carousel advances (if you have images)
- ✅ Mobile menu works (resize browser)
- ✅ All sections display properly

### 7. Configure Custom Domain DNS

**In your DNS provider (where dunamisnexus.net is registered):**

Add a CNAME record:
```
Type: CNAME
Host: lan
Value: yourusername.github.io
TTL: 3600
```

**Wait:** DNS changes take 1-48 hours to propagate.

### 8. Add Custom Domain to GitHub

Once DNS is set up:
1. Back in **Settings** → **Pages**
2. **Custom domain** field: `lan.dunamisnexus.net`
3. Click **Save**
4. Check **Enforce HTTPS** (after DNS propagates)

---

## ⏰ What You Can Do Right Now (While Waiting for DNS):

### A. Customize Content
- Write your About section text
- Add/modify FAQ questions
- Update schedule with your event times
- Customize rules for your venue

### B. Gather Images
- Take photos from past events
- Create or find your logo
- Get permission to use attendee photos
- Resize images to recommended sizes (see README.md)

### C. Set Up Registration
**Option 1: Google Forms**
1. Go to forms.google.com
2. Create new form
3. Add fields: Name, Email, Discord ID, Game Preferences, etc.
4. Click Send → Embed → Copy iframe code
5. Paste in index.html (line ~144, see instructions in HTML file)

**Option 2: LANReg or Similar**
1. Create account on registration platform
2. Create your event
3. Copy event registration URL
4. Add to index.html (line ~151)

### D. Prepare Social Media
- Announce the new site on Discord
- Post on your Mastodon
- Create forum thread about upcoming events
- Share registration opening date

---

## 📋 Pre-Launch Checklist

Before officially promoting your site:

**Content:**
- [ ] Tagline added
- [ ] Event information updated (or marked as TBA)
- [ ] About section customized
- [ ] Schedule updated
- [ ] FAQ reviewed and updated
- [ ] Rules reviewed and updated

**Links:**
- [ ] Discord invite tested
- [ ] Main site link works
- [ ] Forum link works
- [ ] Mastodon link works
- [ ] Ko-fi link works
- [ ] Store link works
- [ ] PayPal link works (if added)

**Images:**
- [ ] Logo added
- [ ] At least 2-3 gallery images added
- [ ] Hero background added (or skipped intentionally)

**Technical:**
- [ ] GitHub Pages enabled
- [ ] Custom domain DNS configured
- [ ] HTTPS enforced
- [ ] Mobile responsive tested
- [ ] All browsers tested (Chrome, Firefox, Safari)

**Registration:**
- [ ] Registration form/link configured
- [ ] Capacity limits set (if applicable)
- [ ] Payment method decided

---

## 🎯 Launch Day Actions

When you're ready to go live:

1. **Final Test**: Visit your site one more time, test everything
2. **Announce on Discord**: Pin a message with the new URL
3. **Forum Post**: Create announcement thread
4. **Social Media**: Share on Mastodon
5. **Email**: Send to your mailing list (if you have one)
6. **Main Site**: Add link from dunamisnexus.net

---

## 🆘 Common Issues & Quick Fixes

**"My images aren't showing!"**
- Check file paths (case-sensitive!)
- Ensure images are committed to GitHub
- Wait a minute and hard refresh (Ctrl+F5)

**"Custom domain shows 404"**
- DNS takes time (up to 48 hours)
- Check CNAME file is in root of repo
- Verify DNS record is correct

**"Carousel not working"**
- Need at least 2 images in gallery folder
- Check JavaScript console for errors
- Ensure script.js is uploaded

**"Mobile menu stuck open"**
- Hard refresh the page
- Check script.js is loaded correctly

---

## 📞 Need Help?

1. Re-read the README.md (comprehensive guide)
2. Check GitHub Pages documentation
3. Ask in Dunamis Nexus Discord #tech-support
4. Google the specific error message

---

## 🎉 Once Live

Congrats! Your site is live. Now:

1. **Monitor registration numbers**
2. **Update event info as it's finalized**
3. **Add more gallery images after each event**
4. **Collect feedback from users**
5. **Keep content fresh and updated**

---

**Remember:** This is YOUR site now. Customize it, make it reflect your community, and have fun with it!

Building Community Through Faith and Gaming 🎮✨
