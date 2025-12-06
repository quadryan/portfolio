# 🚀 Quick Start Guide

## What I've Built For You

Your portfolio is now converted to Astro with:
- ✅ Multi-page structure with routing
- ✅ Reusable layout (nav + footer)
- ✅ All your existing styles in global.css
- ✅ 7 main pages already created
- ✅ 1 detailed project case study (Kleep)

## Immediate Next Steps

### 1. Copy This Folder to Your Repo
```bash
# Copy the entire portfolio-astro folder to your existing repo
cp -r portfolio-astro/* /path/to/your/repo/
```

### 2. Install Dependencies
```bash
cd /path/to/your/repo
npm install
```

### 3. Copy Your Images
Move all your images to the `public/` folder:
```bash
# Your images should be in public/ not src/
# Example:
public/
  ├── airwallex_logo.png
  ├── shopee_logo.png
  ├── MyPhoto.png
  ├── kleep_logo.png
  └── ... (all other images)
```

### 4. Run Development Server
```bash
npm run dev
```

Visit `http://localhost:4321` to see your site!

## Pages Already Created

1. **/** - Homepage with overview
2. **/experience** - All your internships
3. **/projects** - Projects overview
4. **/projects/kleep** - Kleep AI detailed case study
5. **/skills** - Skills & Leadership
6. **/accolades** - Awards & Recognition
7. **/about** - Volunteering & Interests

## Pages You Still Need to Create

I've set up the structure, but you'll need to create:

1. **/projects/shopee** - Shopee UX case study
2. **/projects/fintech-summit** - NUS Fintech Summit case study
3. **/projects/mealmate** - MealMate app details

### How to Create Them

Just copy the `src/pages/projects/kleep.astro` file and modify the content!

```bash
# Example:
cp src/pages/projects/kleep.astro src/pages/projects/shopee.astro
# Then edit shopee.astro with Shopee-specific content
```

## File Structure Explained

```
your-repo/
├── public/               ← Put ALL images here
├── src/
│   ├── layouts/
│   │   └── BaseLayout.astro   ← Nav + Footer (edit once, applies everywhere)
│   ├── pages/
│   │   ├── index.astro        ← Homepage
│   │   ├── experience.astro   ← Experience page
│   │   └── ...                ← Other pages
│   └── styles/
│       └── global.css         ← All your styles
├── astro.config.mjs      ← Astro configuration
└── package.json          ← Dependencies
```

## Editing the Navigation

To add/remove/change nav links, edit:
`src/layouts/BaseLayout.astro`

Look for this section:
```html
<div class="nav-links">
    <a href="/" class="nav-link">Home</a>
    <a href="/experience" class="nav-link">Experience</a>
    <!-- Add your links here -->
</div>
```

## Customizing Styles

All styles are in `src/styles/global.css`. Change colors, fonts, spacing there.

Example:
```css
/* Change primary color from blue to purple */
.nav-link:hover {
    color: #8b5cf6;  /* was #0366d6 */
}
```

## Building for Production

```bash
npm run build
```

This creates a `dist/` folder with your static site.

## Deployment Options

### Option 1: GitHub Pages
1. Build: `npm run build`
2. Push the `dist/` folder to `gh-pages` branch

### Option 2: Netlify
1. Connect your GitHub repo
2. Build command: `npm run build`
3. Publish directory: `dist`

### Option 3: Vercel
Same as Netlify!

## Common Issues & Fixes

### Issue: Images not showing
**Fix:** Make sure images are in `public/` folder, not `src/`

### Issue: Page not found
**Fix:** Check the file exists in `src/pages/` with `.astro` extension

### Issue: Styles not applying
**Fix:** The import in BaseLayout should be:
```html
<link rel="stylesheet" href="/src/styles/global.css">
```

## Need More Help?

Let me know if you need:
- Help creating the remaining project pages
- Style customization
- Deployment assistance
- Any other features!

## Testing Checklist

Before deploying:
- [ ] All images load correctly
- [ ] All navigation links work
- [ ] Mobile responsive (test in DevTools)
- [ ] Content is up to date
- [ ] Contact links work
- [ ] External links open in new tabs

---

**You're ready to go! 🎉**

Run `npm run dev` and start exploring your new multi-page portfolio!
