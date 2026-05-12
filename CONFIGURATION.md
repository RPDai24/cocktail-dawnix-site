# CocktailCouple Website Configuration

## Quick Update Reference

This file documents all the key content that can be easily updated without modifying code structure.

---

## 🔗 Important Links

### Contact Email
- **Current**: support@dawnix.co.uk
- **Used in**: Privacy section, Terms section, Footer
- **How to change**: Find & Replace `support@dawnix.co.uk` → new email

### App Store URL
- **Current**: https://apps.apple.com/app/cocktailcouple
- **Used in**: Hero CTA button, Download section, Footer
- **Status**: **⚠️ NOT LIVE YET** - Update when app is released on App Store
- **How to change**: Find & Replace the URL with actual App Store link

### Company Website
- **Current**: https://dawnix.co.uk
- **Used in**: Footer links
- **Note**: This domain hosts the current website

### Privacy Policy Link
- **Format**: Anchor link `#privacy-section`
- **Location**: Navigation menu, Footer
- **Content location**: Search for `<!-- ========== PRIVACY SECTION ========== -->`

### Terms of Service Link
- **Format**: Anchor link `#terms-section`
- **Location**: Navigation menu, Footer
- **Content location**: Search for `<!-- ========== TERMS SECTION ========== -->`

---

## 🎨 Brand Settings

### Primary Brand Color
- **Current Color**: `#FF7A00` (Orange)
- **CSS Location**: Line ~25 in `<style>` tag: `--primary-orange: #FF7A00;`
- **Used for**: Buttons, links, accents throughout
- **Change it**: Modify hex value, all elements update automatically

### Logo/Brand Name
- **Current**: "CocktailCouple"
- **Navigation bar**: Top-left corner
- **Used in**: Hero, Footer, Meta tags
- **Consistent across**: All sections

---

## 📸 Feature Images & Assets

### Assets Folder Location
`/Users/hupochuan/Work/Coctail Dawnix Website/Assets/`

### Current Images

| Image | Feature | Size* | Status |
|-------|---------|-------|--------|
| Discover.png | Hero + Feature 1 | 1080x1920 | Active |
| Search.png | Feature 2 | 1080x1920 | Active |
| My Bar - Front Bar.png | Feature 3 | 1080x1920 | Active |
| Profile.png | Feature 4 | 1080x1920 | Active |
| My Bar - Storage Back.png | Backup | 1080x1920 | Optional |

*Recommended minimum for sharp display on all devices

### How to Replace an Image

1. **Prepare new image**: Name it clearly, save as PNG
2. **Add to Assets folder**: Copy file to `./Assets/` 
3. **Update HTML reference**:
   ```html
   <img src="./Assets/OLDNAME.png" alt="Old description">
   <!-- Change to: -->
   <img src="./Assets/NEWNAME.png" alt="New description">
   ```
4. **Update alt text**: Make it descriptive for accessibility
5. **Test on mobile & desktop**: Make sure it displays correctly
6. **Commit & push**: Use git to save changes

---

## 📝 Content Sections

### 1. Navigation Menu
- **Location**: Top sticky bar
- **Items**: Features, Download, Privacy, Terms
- **Mobile**: Hamburger menu automatically shows on small screens

### 2. Hero Section
```
Title:       "CocktailCouple"
Subtitle:    "Your Personal Cocktail Companion"
Description: "Discover, search, and craft..."
CTA Buttons: "Download on App Store" | "Learn More"
Image:       ./Assets/Discover.png
```

**To update**: Search for `<!-- ========== HERO SECTION ========== -->`

### 3. Features Section (4 Core Features)

#### Feature 1: Discover
```
Title:       "Discover"
Description: "Browse our extensive collection..."
Image:       ./Assets/Discover.png
Bullets:     • 500+ verified cocktail recipes
             • Classic to contemporary drinks
             • Detailed technique guides
```

#### Feature 2: Smart Search & Filter
```
Title:       "Smart Search & Filter"
Description: "Find the perfect cocktail in seconds..."
Image:       ./Assets/Search.png
Bullets:     • Multi-dimensional search filters
             • Find by ingredients you have
             • Flavor & preparation filters
```

#### Feature 3: My Bar
```
Title:       "My Bar"
Description: "Track all your spirits, liqueurs..."
Image:       ./Assets/My Bar - Front Bar.png
Bullets:     • Inventory management
             • Makeable cocktail suggestions
             • Smart recommendations
```

#### Feature 4: Profile & Favorites
```
Title:       "Profile & Favorites"
Description: "Save your favorite recipes..."
Image:       ./Assets/Profile.png
Bullets:     • Save favorite recipes
             • Custom collections
             • Personal mixology statistics
```

### 4. Highlights Section (Why Choose)

Three columns with icons:
- ⭐ Curated Content - "Every recipe is hand-tested..."
- 🧩 Intelligent Recommendations - "Get personalized suggestions..."
- 👥 Community Focused - "Connect with mixologists..."

### 5. Download Section
```
Title:       "Ready to Elevate Your Cocktail Game?"
Description: "Download CocktailCouple now..."
Button:      "Download on App Store" (links to App Store)
```

### 6. Legal Sections

#### Privacy Policy
- **Sections**: 5 subsections (Info Collection, Usage, Storage, Third-Party, Contact)
- **Email**: support@dawnix.co.uk (configurable)
- **Date**: "Effective Date: May 2024"

#### Terms of Service
- **Sections**: 6 subsections (License, Warranties, Conduct, Liability, Modifications, Contact)
- **Email**: support@dawnix.co.uk (configurable)
- **Date**: "Effective Date: May 2024"

### 7. Footer
```
Column 1: Company info + brief description
Column 2: Product links (Features, Download, App Store)
Column 3: Legal links (Privacy, Terms)
Column 4: Contact (Email, Website)
Copyright: "© 2024 CocktailCouple by Dawnix Ltd"
```

---

## 🔐 Update Procedures

### To Change Email Address
1. **Find**: `support@dawnix.co.uk`
2. **Replace with**: new email
3. **Locations**: Privacy (section 5), Terms (section 6), Footer
4. **Search command**: Ctrl+F in VS Code → type email → replace all

### To Change App Store URL
1. **Find**: `https://apps.apple.com/app/cocktailcouple`
2. **Replace with**: actual App Store URL
3. **Locations**: Hero CTA, Download Section CTA, Footer
4. **Important**: Only change when app is actually live

### To Update Yearly Copyright
1. **Find**: `© 2024 CocktailCouple`
2. **Replace with**: `© 2025 CocktailCouple` (etc.)
3. **Location**: Footer copyright line

### To Update Feature Descriptions
1. **Find**: `<!-- Feature X: [Name] -->` comment
2. **Edit**:
   - `<h3>` = Feature title
   - `<p>` = Feature description
   - `<li>` items = Bullet points
3. **Keep**: HTML structure and classes the same

---

## 📊 Analytics & Monitoring

### Future Enhancement
When ready to add analytics, update:
```html
<!-- Add Google Analytics tag in <head> -->
<script async src="https://www.googletagmanager.com/gtag/..."></script>
```

---

## 🚀 Deployment Steps

### After Making Changes
```bash
# 1. Navigate to project folder
cd '/Users/hupochuan/Work/Coctail Dawnix Website'

# 2. Check what changed
git status

# 3. Stage changes
git add .

# 4. Create descriptive commit message
git commit -m "Update: [what changed]"
# Examples:
# - "Update: Change primary color to blue"
# - "Update: Add new feature description"
# - "Update: Replace app screenshots"

# 5. Push to GitHub (auto-deploys to dawnix.co.uk)
git push origin main

# 6. Wait 1-2 minutes, then verify at https://dawnix.co.uk
```

---

## ✅ Common Update Checklist

### Monthly Reviews
- [ ] Check all external links still work
- [ ] Verify images load correctly
- [ ] Test on latest browsers (Chrome, Safari, Firefox)

### Quarterly Reviews
- [ ] Review privacy/terms for legal changes needed
- [ ] Check if App Store link needs updating
- [ ] Test on new device types (iPad, new phones)
- [ ] Review user feedback if available

### Yearly Updates
- [ ] Update copyright year
- [ ] Review overall design if needed
- [ ] Check if features in description match current app
- [ ] Plan any major content updates

---

## 📋 File Structure Reference

```
Coctail Dawnix Website/
├── index.html                    ← Main website (all content)
├── MAINTENANCE_GUIDE.md          ← How to maintain (this file's sibling)
├── CONFIGURATION.md              ← Quick reference (this file)
├── .gitignore                    ← Git ignore rules
├── CNAME                         ← Domain mapping
├── Assets/
│   ├── Discover.png
│   ├── Search.png
│   ├── My Bar - Front Bar.png
│   ├── Profile.png
│   └── My Bar - Storage Back.png
└── .git/                         ← Git repository
```

---

## 🆘 Quick Troubleshooting

| Problem | Solution |
|---------|----------|
| Changes not appearing | Hard refresh: Cmd+Shift+R (Mac) or Ctrl+Shift+R (Windows) |
| Images broken on mobile | Check image size, ensure PNG format, path: ./Assets/filename.png |
| Links not working | Verify href path (anchor links use #section-id format) |
| Mobile menu stuck | Reload page or use browser DevTools to reset |
| Styles look weird | Wait 10 seconds for Tailwind CDN to load |
| Can't find text to edit | Use Ctrl+F (Find) in editor to search for unique text |

---

**Last Updated**: May 2026  
**Next Review**: August 2026  
**Contact**: support@dawnix.co.uk
