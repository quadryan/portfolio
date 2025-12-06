# Ryan Darius Lim - Portfolio (Astro)

A multi-page portfolio website built with Astro, featuring professional experience, UX case studies, and projects.

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ installed
- Your existing portfolio images and assets

### Installation

1. **Install dependencies:**
```bash
npm install
```

2. **Run development server:**
```bash
npm run dev
```

Your site will be available at `http://localhost:4321`

3. **Build for production:**
```bash
npm run build
```

4. **Preview production build:**
```bash
npm run preview
```

## 📁 Project Structure

```
portfolio-astro/
├── public/              # Static assets (images, logos)
│   ├── airwallex_logo.png
│   ├── shopee_logo.png
│   ├── MyPhoto.png
│   └── ... (all your other images)
├── src/
│   ├── layouts/
│   │   └── BaseLayout.astro    # Main layout with nav + footer
│   ├── pages/
│   │   ├── index.astro         # Homepage
│   │   ├── experience.astro    # Professional experience
│   │   ├── projects.astro      # Projects overview
│   │   ├── projects/
│   │   │   ├── kleep.astro     # Kleep case study
│   │   │   ├── shopee.astro    # (to be created)
│   │   │   ├── fintech-summit.astro # (to be created)
│   │   │   └── mealmate.astro  # (to be created)
│   │   ├── skills.astro        # (to be created)
│   │   ├── accolades.astro     # (to be created)
│   │   └── about.astro         # (to be created)
│   └── styles/
│       └── global.css          # All your existing styles
├── astro.config.mjs
└── package.json
```

## 🔄 Migration Steps

### Step 1: Copy Your Images
Move all your images from your old portfolio to the `public/` folder:
```bash
# From your old repo
cp *.png /path/to/portfolio-astro/public/
cp *.jpg /path/to/portfolio-astro/public/
```

### Step 2: Update Configuration
In `astro.config.mjs`, update the site URL:
```js
site: 'https://yourusername.github.io'
```

### Step 3: Create Remaining Pages
I've created the core structure. You still need to create:
- `src/pages/skills.astro` - Skills & Leadership page
- `src/pages/accolades.astro` - Accolades & Recognition
- `src/pages/about.astro` - About, Volunteering, Interests
- `src/pages/projects/shopee.astro` - Shopee UX case study
- `src/pages/projects/fintech-summit.astro` - Fintech Summit case study
- `src/pages/projects/mealmate.astro` - MealMate project

I can help you create these! Just let me know.

## 📄 Pages & Routes

- `/` - Homepage with overview
- `/experience` - All professional experience
- `/projects` - Projects overview
- `/projects/kleep` - Kleep AI case study
- `/projects/shopee` - Shopee UX case study (to be created)
- `/projects/fintech-summit` - NUS Fintech Summit (to be created)
- `/projects/mealmate` - MealMate app (to be created)
- `/skills` - Skills & Leadership (to be created)
- `/accolades` - Accolades & Recognition (to be created)
- `/about` - About & Volunteering (to be created)

## 🎨 Customization

### Editing Styles
All styles are in `src/styles/global.css`. Modify this file to update colors, fonts, spacing, etc.

### Adding New Pages
1. Create a new `.astro` file in `src/pages/`
2. Import and use the `BaseLayout`
3. Add navigation link in `src/layouts/BaseLayout.astro`

Example:
```astro
---
import BaseLayout from '../layouts/BaseLayout.astro';
---

<BaseLayout title="Your Page Title">
    <div class="section" style="padding-top: 80px;">
        <div class="container">
            <!-- Your content here -->
        </div>
    </div>
</BaseLayout>
```

## 🚢 Deployment

### GitHub Pages
1. Update `astro.config.mjs` with your repo name
2. Build: `npm run build`
3. Deploy the `dist/` folder to GitHub Pages

### Netlify/Vercel
1. Connect your GitHub repo
2. Build command: `npm run build`
3. Publish directory: `dist`

## ✅ What's Been Created

- ✅ Base layout with navigation and footer
- ✅ Global CSS (all your existing styles)
- ✅ Homepage with overview
- ✅ Professional Experience page
- ✅ Projects overview page
- ✅ Kleep AI case study page
- ⏳ Shopee case study (template ready, needs content)
- ⏳ Fintech Summit case study (template ready, needs content)
- ⏳ MealMate project page (template ready, needs content)
- ⏳ Skills & Leadership page
- ⏳ Accolades page
- ⏳ About page

## 💡 Next Steps

1. Copy all your images to the `public/` folder
2. Run `npm install` and `npm run dev` to test
3. Let me know which remaining pages you want me to create next!
4. Customize colors/styles if needed
5. Deploy to your hosting platform

## 🆘 Need Help?

Let me know if you need help with:
- Creating the remaining pages
- Customizing styles
- Adding new features
- Deployment configuration
