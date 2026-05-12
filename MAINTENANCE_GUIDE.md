# CocktailCouple Website Maintenance Guide

## 📋 Quick Overview

This is a static website built with **HTML5 + Tailwind CSS** (via CDN). No build process or dependencies needed.

- **Framework**: Tailwind CSS (CDN link)
- **Hosting**: GitHub Pages (automatic deployment)
- **Domain**: https://dawnix.co.uk (via CNAME file)
- **Source**: `/Users/hupochuan/Work/Coctail Dawnix Website/index.html`

---

## 🎨 Design System

### Color Scheme
```css
Primary Orange:    #FF7A00    /* Used for links, buttons, accents */
White Background:  #ffffff    /* Main page background */
Light Background:  #f8f9fa    /* Section alternating backgrounds */
Dark Background:   #111111    /* Footer background */
Text Colors:       Gray shades (gray-600, gray-900, etc.)
```

### Breakpoints (Responsive)
- **Mobile**: < 768px (md breakpoint)
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px (lg breakpoint)

**How to use**: Classes like `md:grid-cols-2` apply at tablet+ sizes. `hidden md:flex` hides on mobile, shows on tablet+.

---

## 📁 Asset Management

### Current Assets in `./Assets/`
```
Assets/
├── Discover.png                    (Hero + Feature 1)
├── Search.png                      (Feature 2)
├── My Bar - Front Bar.png          (Feature 3)
├── Profile.png                     (Feature 4)
└── My Bar - Storage Back.png       (Optional backup)
```

### How to Replace Images

1. **Add new image** to `./Assets/` folder
2. **Find the image reference** in index.html (search filename)
3. **Update the src attribute**:
   ```html
   <!-- Before -->
   <img src="./Assets/Discover.png" alt="Old description">
   
   <!-- After -->
   <img src="./Assets/NewImage.png" alt="New description">
   ```
4. **Update alt text** for accessibility
5. **Test responsiveness** on mobile/desktop
6. **Commit & push** to GitHub

### Image Optimization Tips
- Use **PNG for crisp screenshots** (current format)
- Keep resolution **1080x1920px minimum** (mobile-friendly)
- Compress if file size > 500KB (use https://tinypng.com)
- Use consistent aspect ratios across feature images

---

## ✏️ Content Updates

### Update Text Content

All text is organized by **sections**. Search for section comments in index.html:

```
<!-- ========== NAVIGATION ========== -->
<!-- ========== HERO SECTION ========== -->
<!-- ========== FEATURES SECTION ========== -->
<!-- ========== HIGHLIGHTS SECTION ========== -->
<!-- ========== DOWNLOAD SECTION ========== -->
<!-- ========== PRIVACY SECTION ========== -->
<!-- ========== TERMS SECTION ========== -->
<!-- ========== FOOTER ========== -->
```

### Common Changes

#### 1. Update App Store Link
- **Find**: `href="https://apps.apple.com/app/cocktailcouple"`
- **Change**: Replace with actual App Store URL once app is live
- **Locations**: Hero CTA, Download Section, Footer

#### 2. Update Email Address
- **Current**: `support@dawnix.co.uk`
- **Find & Replace**: `support@dawnix.co.uk` with new email
- **Locations**: Privacy section, Terms section, Footer

#### 3. Update Feature Descriptions
- **Location**: Features Section → Find `<h3>` heading and `<p>` paragraphs
- **Change**: Update feature titles and descriptions
- **Keep**: HTML structure (li items with checkmarks) - same pattern

#### 4. Update Company Info
- **Location**: Footer
- **Change**: "© 2024 CocktailCouple by Dawnix Ltd" if needed
- **Date**: Update year when website is refreshed

---

## 🔧 Customization Guide

### Change the Brand Color

1. **Find in CSS** (around line 25):
   ```css
   :root {
       --primary-orange: #FF7A00;    /* Change this */
   }
   ```

2. **Change hex value**: Replace `#FF7A00` with new color
3. **All elements update automatically** (buttons, links, accents)
4. **Test**: Check on different sections to ensure readability

### Modify Section Layouts

Each feature uses a responsive grid:
```html
<div class="grid md:grid-cols-2 gap-8 items-center">
    <!-- Left: Image or Content -->
    <!-- Right: Content or Image -->
</div>
```

- `md:grid-cols-2` = 2 columns on tablet+, 1 on mobile
- `gap-8` = spacing between columns (adjust to gap-4, gap-12, etc.)
- `items-center` = vertically center content (remove if not needed)

### Add New Feature

1. **Copy existing feature block** (find `<!-- Feature X -->` section)
2. **Paste after last feature**
3. **Update**:
   - Feature number (Feature 5, etc.)
   - Image path: `./Assets/NewImage.png`
   - Title: `<h3>New Feature Name</h3>`
   - Description: `<p>Feature description...</p>`
   - Bullet points: Update `<li>` items
4. **Maintain order class** for desktop: `order-1 md:order-2` (alternates image position)

---

## 📱 Testing Checklist

### Before Publishing Changes

- [ ] Desktop view (1200px+) looks correct
- [ ] Tablet view (768px-1023px) responsive and readable
- [ ] Mobile view (320px-767px) text scales, images fit
- [ ] All links work (test each href)
- [ ] Images load (no 404 errors)
- [ ] Colors look good (contrast for readability)
- [ ] Smooth scrolling works (anchor links)
- [ ] Mobile menu opens/closes properly
- [ ] No console errors (open DevTools: F12)

### How to Test Locally

1. **Open index.html in browser**: File → Open File → select index.html
2. **Open DevTools**: Press F12
3. **Toggle device toolbar**: Click phone icon (top-left of DevTools)
4. **Test responsive**: Adjust width, switch between devices

---

## 🚀 Deployment

### Automatic Deployment
- **Push to GitHub**: Changes to `main` branch auto-deploy to GitHub Pages
- **Timing**: Usually live within 1-2 minutes
- **Domain**: https://dawnix.co.uk (configured via CNAME)

### Manual Deployment (if needed)
```bash
cd '/Users/hupochuan/Work/Coctail Dawnix Website'
git add .
git commit -m "Update: [describe changes]"
git push origin main
```

### Verify Deployment
1. Wait 1-2 minutes after push
2. Visit https://dawnix.co.uk
3. Refresh with Ctrl+Shift+R (hard refresh to clear cache)
4. Check on mobile too (use Chrome DevTools device toggle)

---

## 📝 SEO & Metadata

### Update Meta Tags (in `<head>`)

```html
<!-- Page title (appears in browser tab & search results) -->
<title>CocktailCouple - Your Personal Cocktail Companion</title>

<!-- Search engine description (shows under link) -->
<meta name="description" content="...">

<!-- Social media preview -->
<meta property="og:title" content="...">
<meta property="og:description" content="...">
<meta property="og:image" content="./Assets/Discover.png">
```

### SEO Tips
- Keep title under 60 characters
- Description under 160 characters
- Keywords separated by commas (but not critical for Google)
- og:image should be a 1200x630px image for best preview

---

## ❓ Troubleshooting

### Images Not Showing
1. Check filename spelling in `./Assets/` folder
2. Verify correct path: `./Assets/Filename.png`
3. Open DevTools (F12) → Check Console tab for 404 errors

### Styles Look Broken
1. Tailwind CDN might be slow to load
2. Try hard refresh: **Ctrl+Shift+R** (Windows/Linux) or **Cmd+Shift+R** (Mac)
3. Wait 10 seconds for Tailwind to process

### Mobile Menu Stuck
1. Open DevTools → Console
2. Type: `document.getElementById('mobileMenu').classList.add('hidden')`
3. Press Enter
4. Check code - ensure JavaScript at bottom is intact

### Changes Not Live
1. Check you're on `main` branch: `git branch`
2. Verify push succeeded: `git log --oneline` (should see your commit)
3. Hard refresh website: **Cmd+Shift+R** (Mac)
4. Wait 2-3 minutes for GitHub Pages to rebuild

---

## 📊 Performance Tips

- **Images**: Keep under 500KB each (compress at https://tinypng.com)
- **CSS**: Tailwind CDN is fast enough for small sites
- **JavaScript**: Minimal JS (only mobile menu toggle) = fast page
- **Caching**: GitHub Pages caches aggressively - hard refresh if updates don't show

---

## 📞 Support Contacts

- **Email**: support@dawnix.co.uk
- **Website**: https://dawnix.co.uk
- **Repository**: Check git history for past changes

---

## 🔄 Update History

| Date | Changes |
|------|---------|
| May 2024 | Initial English website launch with 4 core features, Privacy & Terms integrated, responsive design |
| - | Future updates will be logged here |

---

## ✅ Maintenance Checklist (Quarterly)

- [ ] Test all links still work
- [ ] Verify images load correctly
- [ ] Check App Store link (update if new version)
- [ ] Review privacy/terms for legal updates needed
- [ ] Test on different browsers (Chrome, Safari, Firefox)
- [ ] Check mobile compatibility one more time
- [ ] Review analytics (if implemented later)

---

**Last Updated**: May 2024  
**Maintainer**: CocktailCouple Team  
**Questions?** Contact: support@dawnix.co.uk
