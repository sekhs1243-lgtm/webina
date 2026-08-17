# Webina — Professional Web Solutions

A high-performance, responsive, and deployment-ready website for **Webina**, a web development company specializing in custom web applications, business websites, e-commerce, and shop management systems.

---

## 🚀 Features

- **Pure Static Architecture:** Zero build steps, zero bloated dependencies, ultra-fast initial load times.
- **Production-Compiled CSS:** Tailored typography with Google Fonts (*Cormorant* & *Work Sans*), glassmorphism styling, and noise overlays.
- **Dynamic Interactive Components:**
  - Animated multilingual intro greeting (with accessibility `prefers-reduced-motion` support)
  - Interactive hero typewriter headline
  - Infinite auto-scrolling country flags marquee
  - Infinite auto-scrolling tech stack & feature marquees
  - Filterable/Expandable portfolio showcase modal
  - Quote request modal with pre-selected package details
  - Schedule meeting modal with date/time pickers
  - Responsive tabbed Legal Modal (Privacy Policy & Terms of Service)
  - Floating WhatsApp chat widget & multi-channel contact form (`mailto:` fallback)
  - Multilingual translation support via Google Translate API
- **Enterprise SEO & Structured Data:**
  - Complete Open Graph and Twitter Card tags
  - Valid JSON-LD Schema (`WebSite`, `Organization`, `ProfessionalService`)
  - XML Sitemap (`sitemap.xml`) & `robots.txt`
  - Canonical link tags and DNS prefetch hints

---

## 📁 Project Structure

```text
WebinaFinal/
├── index.html         # Main website markup, styles, structured data, and logic
├── robots.txt         # Search engine crawler instructions
├── sitemap.xml        # XML sitemap for SEO discovery
├── .gitignore         # Standard git exclusion rules
├── README.md          # Project overview, setup, and deployment instructions
└── EDIT-GUIDE.md      # Beginner-friendly guide for updating all website details
```

---

## 💻 Running Locally

You can preview the website locally using any standard static web server or simply by double-clicking `index.html`.

### Option 1: Using Python
```bash
# Python 3
python -m http.server 8000
```
Then open `http://localhost:8000` in your web browser.

### Option 2: Using Node.js
```bash
npx serve .
```

### Option 3: VS Code Live Server
Right-click `index.html` inside VS Code and click **"Open with Live Server"**.

---

## 🌐 Deployment Instructions

Because this is a pure static website, it can be deployed to any modern static hosting provider in seconds without any build commands.

### 1. Netlify (Recommended)
1. Log in to [Netlify](https://app.netlify.com).
2. **Drag and drop** this entire folder (`WebinaFinal`) directly into the Netlify dashboard.
3. Or link your GitHub repository with:
   - **Build command:** *(leave empty)*
   - **Publish directory:** `.` or `/`

### 2. Vercel
1. Install Vercel CLI (optional) or use the dashboard:
   ```bash
   npx vercel
   ```
2. Or import your Git repository in [Vercel](https://vercel.com) and set:
   - **Framework Preset:** `Other`
   - **Build Command:** *(leave empty)*
   - **Output Directory:** `.`

### 3. GitHub Pages
1. Push this repository to GitHub.
2. Navigate to repository **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, select **Deploy from a branch**.
4. Choose branch `main` and folder `/ (root)`, then click **Save**.

### 4. Cloudflare Pages
1. Go to Cloudflare Dashboard > **Workers & Pages** > **Create application** > **Pages**.
2. Connect your Git repository.
3. Set **Build command** to *(none)* and **Output directory** to `.`.

---

## ✏️ How to Edit Information

See [`EDIT-GUIDE.md`](./EDIT-GUIDE.md) for a comprehensive line-by-line guide on updating:
- Email address & WhatsApp phone number
- Project cards, screenshots & demo URLs
- Pricing packages, features & delivery times
- Country flags & technologies list
- Privacy Policy & Terms of Service document links
- Page title & SEO meta tags
