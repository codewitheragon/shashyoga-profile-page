# Yoga with Shashi — Profile Page

An authentic, bilingual (English & Hindi) profile page for Shashi Shastri, a Master in Hatha Yoga. Built with **Astro** and **Tailwind CSS v4** for high performance and easy customization.

## 🚀 Project Overview

This project is a refactored version of the original single-page website. It utilizes a modern component-based architecture to separate content from structure, making it "neatly customizable" for future updates.

### Key Features
- **Bilingual Support**: Instant, zero-reload switching between English and Hindi.
- **Component-Based**: UI is broken down into reusable Astro components.
- **Data-Driven**: All text content is centralized in a single TypeScript file.
- **Optimized Performance**: Static site generation with minimal client-side JavaScript.
- **Tailwind CSS v4**: Modern styling with a custom "Forest & Cream" palette.

---

## 🏗️ Architecture

The project follows a modular structure:

- **`src/layouts/`**: Contains the main `Layout.astro` which handles SEO meta tags, Google Fonts, and the language switching logic.
- **`src/components/`**: Individual UI sections:
    - `Navbar.astro`: Sticky navigation with language toggle.
    - `Hero.astro`: Entry section with CTA buttons and proof badges.
    - `About.astro`: The "From the Mat" narrative and core credentials timeline.
    - `Gallery.astro`: Visual showcase of practice and YouTube links.
    - `Dimensions.astro`: Detailed expertise (Patanjali, Shatkarma) and contact banner.
    - `Testimonials.astro`: Student chronicles and social proof.
    - `Footer.astro`: Social links and copyright.
- **`src/data/`**: The heart of the customization.
    - `content.ts`: Stores every string, paragraph, and link used across the site in both languages.

---

## 🛠️ How to Customize

To change any text, testimonials, or links on the site, you do **not** need to touch the HTML components. Simply edit:

`src/data/content.ts`

The schema is structured by section, for example:
```typescript
hero: {
  title: {
    en: "Embrace the Authentic Path...",
    hi: "योग के प्रामाणिक मार्ग..."
  }
}
```

---

## 💻 Development Commands

All commands are run from the root of the project, using a terminal:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs dependencies |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `npm run build` | Build your production site to `./dist/` |
| `npm run preview` | Preview your build locally before deploying |

---

## 🌐 Deployment

This project is optimized for static hosting. You can deploy the generated `dist/` folder to:
- Cloudflare Pages
- Netlify
- Vercel
- GitHub Pages

**Build Settings:**
- **Build Command:** `npm run build`
- **Output Directory:** `dist`
