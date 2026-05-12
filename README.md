# CocktailCouple Official Website

**Professional Landing Page for iOS App**  
🌐 Live at: https://dawnix.co.uk  
📱 App: CocktailCouple on App Store

---

## 📖 Overview

This is a **long-term maintainable** landing website for the **CocktailCouple** iOS app. Built with clean HTML5 + Tailwind CSS, designed for:

✅ **Easy Content Updates** - Change text, images, and links without coding knowledge  
✅ **Responsive Design** - Works perfectly on mobile, tablet, desktop  
✅ **Fast & Lightweight** - No build process, no dependencies, quick load times  
✅ **SEO Ready** - Proper meta tags, semantic HTML, mobile-optimized  
✅ **Zero Maintenance** - Static HTML, hosted free on GitHub Pages  

---

## 🎯 Purpose & Sections

The website showcases the CocktailCouple app with:

1. **Hero Section** - App headline, tagline, download CTA
2. **4 Core Features** - Discover, Search, My Bar, Profile (with screenshots)
3. **Why Choose Us** - Curated content, smart recommendations, community focus
4. **Download CTA** - App Store download button
5. **Legal Pages** - Privacy Policy & Terms of Service (integrated, no separate files)
6. **Footer** - Company info, links, contact

---

## 📁 Project Structure

```
Coctail Dawnix Website/
│
├── 📄 index.html                    # Main website (single HTML file)
│   ├── Head: Meta tags, SEO, styling (Tailwind CDN)
│   ├── Body: Navigation, 7 sections, footer
│   └── Script: Mobile menu toggle (5 lines of JS)
│
├── 📚 Documentation (for maintenance)
│   ├── README.md                    # This file
│   ├── MAINTENANCE_GUIDE.md         # Detailed how-to guide
│   └── CONFIGURATION.md             # Content & settings reference
│
├── 🖼️ Assets/
│   ├── Discover.png                 # App screenshots
│   ├── Search.png
│   ├── My Bar - Front Bar.png
│   ├── Profile.png
│   └── My Bar - Storage Back.png
│
├── 🔧 Git & Deployment
│   ├── .gitignore                   # Ignore unnecessary files
│   ├── CNAME                        # Domain mapping for GitHub Pages
│   └── .git/                        # Git history & version control
│
└── 📋 Configuration Files
    └── (GitHub Pages auto-configures from CNAME + repo settings)
```

---

## 🚀 Quick Start

### For First-Time Visitors
1. **Open** https://dawnix.co.uk in browser
2. **View** responsive design - try desktop, tablet, mobile
3. **Test** navigation - smooth scrolling, mobile menu
4. **Check** all links work properly

### For Content Maintainers

**To make updates:**
1. Open `index.html` in any text editor (VS Code, Sublime, etc.)
2. Find the section you want to change (clearly marked with HTML comments)
3. Edit text, images, or links
4. Save file
5. Commit to git & push to GitHub (auto-deploys in 1-2 minutes)

See **MAINTENANCE_GUIDE.md** for detailed instructions.

### For Developers

**To understand the code:**
- Clean HTML5 semantic structure (nav, section, footer)
- Tailwind CSS utility classes (no custom CSS bloat)
- Responsive breakpoints: `md:` (768px+), `lg:` (1024px+)
- Minimal JavaScript (only mobile menu toggle)
- CDN-based (no npm, webpack, or build process)

---

## 📊 Design System

### Colors
| Use | Color | Hex Code |
|-----|-------|----------|
| Primary/Accent | Orange | #FF7A00 |
| Background | White | #ffffff |
| Alt Background | Light Gray | #f8f9fa |
| Dark (Footer) | Dark Gray | #111111 |
| Text Primary | Dark Gray | #111111 |
| Text Secondary | Medium Gray | #666666 |

### Typography
- **Headings**: Bold, sans-serif, hierarchy (7xl → 3xl)
- **Body Text**: Regular weight, readable 18-20px on mobile
- **Links**: Orange with hover underline animation

### Responsive Breakpoints
- **Mobile**: 320px - 767px (hidden: desktop menu)
- **Tablet**: 768px - 1023px (shown: desktop menu, 2-column layouts)
- **Desktop**: 1024px+ (full 3-column layouts, larger spacing)

---

## 🔄 Maintenance Workflow

### Scenario 1: Update Feature Description
```
1. Open index.html
2. Search for: "<!-- Feature 1: Discover -->"
3. Edit <h3> title or <p> description
4. Save, commit, push
5. Done! Live in 1-2 minutes
```

### Scenario 2: Replace App Screenshot
```
1. Add new image to Assets/ folder
2. Open index.html
3. Search for old image filename
4. Change src="./Assets/OldName.png" → "NewName.png"
5. Save, commit, push
6. Done! Live in 1-2 minutes
```

### Scenario 3: Update Privacy Policy
```
1. Open index.html
2. Search for: "<!-- ========== PRIVACY SECTION ========== -->"
3. Edit content under "2. How We Use Your Information" (etc.)
4. Save, commit, push
5. Done! Live in 1-2 minutes
```

### Scenario 4: Change Brand Color
```
1. Open index.html → Find <style> section
2. Search: "--primary-orange: #FF7A00;"
3. Change hex value to new color: "#FF6600" (example)
4. All orange elements update automatically
5. Save, commit, push
6. Done! Live in 1-2 minutes
```

---

## 📋 Content Inventory

### Text Content That Changes Often
- ✅ Feature descriptions
- ✅ Email address (support contact)
- ✅ App Store link (when launching)
- ✅ Privacy policy details
- ✅ Terms of service details
- ✅ Company/copyright info

### Visual Content (Assets)
- ✅ App screenshots (4 current features)
- ✅ Future: Hero image, testimonials, etc.

### Settings (One-Time Setup)
- ⚙️ Brand color (#FF7A00)
- ⚙️ Domain mapping (CNAME → dawnix.co.uk)
- ⚙️ SEO meta tags

---

## 🧪 Quality Assurance

### Pre-Launch Checklist ✅
- [x] Responsive design tested (mobile, tablet, desktop)
- [x] All links functional
- [x] Images load correctly
- [x] No console errors (DevTools)
- [x] Accessibility proper (alt text, semantic HTML)
- [x] Fast page load (static HTML = instant)
- [x] Legal pages complete (Privacy, Terms)
- [x] SEO optimized (meta tags, descriptions)

### Regular Maintenance
- **Weekly**: Spot-check links, images on different devices
- **Monthly**: Verify App Store link works, check email deliverability
- **Quarterly**: Full responsive test across devices, browser compatibility check
- **Yearly**: Update copyright year, review for design refresh

---

## 🔐 Security & Privacy

### Data Handling
- ✅ No form submissions (no user data collected on website)
- ✅ No third-party analytics tracking (can add later if needed)
- ✅ HTTPS only (GitHub Pages enforces)
- ✅ Privacy policy explains app's data collection (not website's)

### Deployment Security
- ✅ Repository is public (code visible, which is fine for static sites)
- ✅ No sensitive credentials in code
- ✅ CNAME protects domain via GitHub Pages
- ✅ Automatic HTTPS certificate via GitHub Pages

---

## 📈 Analytics & Monitoring

### Current State
- No analytics implemented (static HTML, GitHub Pages doesn't track)
- No conversion tracking yet

### For Future
To add Google Analytics:
1. Get tracking ID from Google Analytics
2. Add script tag to `<head>` section
3. Test with DevTools
4. Monitor visitor behavior

---

## 🐛 Troubleshooting

### Website Issues

**Images not showing?**
- Check `./Assets/` folder for correct filename
- Verify path: `src="./Assets/FileName.png"`
- Hard refresh: Cmd+Shift+R (Mac)

**Styles look broken?**
- Tailwind CDN loading might be slow
- Hard refresh: Ctrl+Shift+R (Windows)
- Wait 10 seconds

**Mobile menu stuck?**
- Reload page
- Check browser console for JavaScript errors

**Changes not live?**
- Verify commit pushed: `git log --oneline`
- Wait 2-3 minutes for GitHub Pages rebuild
- Hard refresh website in browser

See **MAINTENANCE_GUIDE.md** for more troubleshooting.

---

## 📚 Documentation Files

| File | Purpose |
|------|---------|
| **README.md** | Overview & quick start (you're reading this) |
| **MAINTENANCE_GUIDE.md** | Detailed how-to for updates, testing, troubleshooting |
| **CONFIGURATION.md** | Content inventory & settings reference |

**Read in order**: README → CONFIGURATION → MAINTENANCE_GUIDE

---

## 🎯 Goals Achieved

### ✅ Maintainability
- Clear HTML comments for each section
- Centralized CSS variables for easy color changes
- Reusable component patterns (cards, buttons, grids)
- Minimal JavaScript (only essentials)
- No complex build process

### ✅ Scalability
- Easy to add new sections (copy/paste existing patterns)
- Responsive design supports all devices
- Asset-agnostic (works with any screenshots)
- Future-proof HTML5 & CSS3 standards

### ✅ Performance
- Lightweight: Single HTML file + 5 PNG images
- Fast load: No external JS libraries (except Tailwind CDN)
- Mobile-optimized: Lazy loading, responsive images
- SEO-ready: Semantic HTML, meta tags, fast speed

### ✅ Professional
- Modern design following iOS-native aesthetic
- Brand color (#FF7A00) consistent throughout
- Legal pages integrated (App Store requirements)
- GitHub Pages deployment (free, automatic)

---

## 📞 Support & Contact

**Questions about the website?**
- Email: support@dawnix.co.uk
- Check: MAINTENANCE_GUIDE.md first
- Review: CONFIGURATION.md for settings

**Found a bug?**
- Describe the issue
- Note browser & device
- Email: support@dawnix.co.uk

---

## 📝 Version History

| Date | Change | Status |
|------|--------|--------|
| May 2024 | Initial launch - English website with 4 features, Privacy/Terms, responsive design | ✅ Live |
| - | Future: Analytics, blog section, testimonials | ⏳ Planned |

---

## 📄 License & Attribution

- **Website Design**: Optimized for CocktailCouple app
- **Framework**: Tailwind CSS (MIT License)
- **Hosting**: GitHub Pages (free)
- **Domain**: dawnix.co.uk (via CNAME)

---

## ✨ Next Steps

### If You're New
1. **Read this README** (overview)
2. **Check CONFIGURATION.md** (understand what can change)
3. **Try MAINTENANCE_GUIDE.md** (make a test change)
4. **Deploy**: Follow deployment steps in MAINTENANCE_GUIDE

### If You're Making Updates
1. **Open index.html** in text editor
2. **Find the section** you want to change (HTML comments mark sections)
3. **Make your edit** (text, image path, link)
4. **Test locally** (open in browser)
5. **Commit & push** to GitHub (auto-deploys)
6. **Verify** at https://dawnix.co.uk (wait 1-2 minutes)

### If You're Deploying
1. Make changes locally
2. Test on mobile & desktop (DevTools device toggle)
3. Run: `git add . && git commit -m "Update: [description]" && git push origin main`
4. Wait 1-2 minutes
5. Verify at https://dawnix.co.uk with Cmd+Shift+R hard refresh

---

## 🎓 Learning Resources

- **HTML5 Semantic Tags**: https://developer.mozilla.org/en-US/docs/Glossary/semantics
- **Tailwind CSS**: https://tailwindcss.com/docs
- **Responsive Design**: https://web.dev/responsive-web-design-basics/
- **GitHub Pages**: https://pages.github.com/

---

**Created**: May 2024  
**Last Updated**: May 2026  
**Maintainer**: CocktailCouple Team  
**Status**: ✅ Production Ready

---

## 💡 Key Principle

> **This website is designed for long-term maintainability.** Anyone on your team should be able to update content (text, images, links) without understanding code. The structure is clear, the comments are detailed, and the documentation covers 99% of common tasks.

**You got this! 🎉**
