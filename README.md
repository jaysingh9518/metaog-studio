# 🔮 MetaOG Studio — OpenGraph & Live SEO Meta Inspector

A high-performance, single-file web studio for designing social share cards (1200×630 landscape & 1080×1080 square) and inspecting live website SEO metadata with real-time Google SERP simulation.

---

## 🌟 Key Features

### 1. 🎨 Social Card Designer (OG Studio)
* **Dual Aspect Ratios**:
  * **Standard Landscape (1200 × 630 px)**: Optimized for Twitter Large Summary cards, Facebook, LinkedIn, Discord, and Slack.
  * **Square (1080 × 1080 px)**: Dedicated 1:1 layout engine with adaptive two-tier capsule pill distribution and auto-wrapped subtitles for Instagram and mobile feeds.
* **Dual Card Themes**:
  * **Dark Card Theme**: Deep midnight/navy background with luminous radial glow and fine blueprint technical grid.
  * **Light Card Theme**: Ultra-clean high-contrast slate backdrop with frosted semi-transparent pill badges and crisp typography.
  * *Note: Card themes operate independently of the app's light/dark user interface.*
* **Logo & Brand Customization Suite**:
  * Upload custom logos (`PNG`, `SVG`, `JPG`, `WebP`) or provide image URLs.
  * **Smart Color Extraction**: Automatically samples dominant brand colors from uploaded logos to sync card backgrounds and accent glows with one click.
  * **Transparency Suite**: Toggle logo background transparency or select from preset chips (`Transparent`, `Brand Primary`, `Navy`, `White`).
  * Comprehensive sizing, inner padding, border radius (square to circle), border thickness, and border line styles (`solid`, `dashed`, `dotted`).
  * Fallback initial badges when no image file is loaded.
* **4 Modular Visual Zone Editing Tabs**:
  * **1. Header**: Logo dimensions, alignments (`Left`, `Center`, `Right`), company name, and subtitle location string.
  * **2. Titles**: Two-tone headline split into Primary Title and Accent Headline Highlight with dedicated tracking, line-height multipliers, and text transform selectors.
  * **3. Features**: Subtitle capabilities line and dynamic **Capsule Pills Manager**.
  * **4. Frame & Spacing**: Contact footer text, card background fill, blueprint grid toggle, outer border toggle, and radial glow toggle.
* **Dynamic Section Spacing Engine**:
  * Interactive sliders to configure pixel-perfect vertical gaps:
    * *Top Canvas Inset*
    * *Header → Title Gap*
    * *Title → Subtitle Gap*
    * *Subtitle → Feature Pills Gap*
  * One-click **Reset Gaps** to restore balanced proportions.
* **Dynamic Capsule Pills Manager**:
  * Add custom feature badges with custom emojis/icons.
  * Delete pills via trash actions or toggle visibility individually.
  * Global pill font styling, weight selection, and text capitalization.
* **Floatable Picture-in-Picture (PiP) Preview**:
  * Toggle between standard embedded **Stacked** layout and a floating **PiP Window**.
  * Move the floating preview anywhere on the screen via the drag handle.
  * Minimize to a compact dock or switch between width presets (`420px`, `520px`, `640px`).
* **Instant Exports**:
  * High-resolution **2× Retina PNG download**.
  * Standalone vector **SVG download**.
  * 1-Click **Copy PNG** directly to the operating system clipboard (via `ClipboardItem`).
  * 1-Click **Copy SVG code**.

---

### 2. 🔍 Live URL & SEO Inspector
* **Live Web Scraper**:
  * Input any public URL (`https://example.com`) to inspect real production `<title>`, `<meta name="description">`, `<link rel="canonical">`, `og:image`, and site name.
  * CORS-resilient multi-proxy fallback architecture (`allorigins.win`, `corsproxy.io`, `codetabs`).
* **Vector SVG OG Image Support**:
  * Capable of rendering vector `.svg` open graph images inline alongside standard raster formats (`PNG`, `JPG`, `WebP`).
* **Real-time SEO Validation Benchmarks**:
  * **Meta Title Tracker**: Calibrated to the recommended **50–60 characters** limit with real-time visual progress meter to prevent SERP truncation.
  * **Meta Description Tracker**: Benchmark targeting **~131 characters** (optimal 120–160 character range) for mobile and desktop SERP visibility.
* **Live Google SERP Simulator**:
  * Toggle between **Desktop** and **Mobile** search result snippets.
* **SEO Health Score**:
  * Automated audit grade percentage and checklist verifying canonical URL security and OG image tags.
* **Send to OG Generator**:
  * 1-Click migration of scraped metadata directly into the Social Card Designer canvas.
* **Production HTML Snippet**:
  * Formatted, copy-ready `<meta>` tags for quick integration into your website's `<head>`.

---

## 🚀 Quick Start & Deployment to GitHub Pages

### Option A: Direct Local Preview
Because MetaOG Studio is built as a single, self-contained file with zero build step dependencies:
1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser.
3. (Optional) Run via local HTTP server:
   ```bash
   npx serve .
   ```

---

### Option B: Deploy to GitHub Pages (Free Hosting)

#### Step 1: Create a GitHub Repository
1. Head to [GitHub.com/new](https://github.com/new) and create a public repository named `metaog-studio`.

#### Step 2: Push Files to GitHub
Run the following commands in your terminal inside the project directory:

```bash
# Initialize git repository
git init

# Add files
git add .

# Commit changes
git commit -m "feat: complete MetaOG studio application with floating preview and SEO inspector"

# Set branch to main
git branch -M main

# Add remote origin (replace YOUR_USERNAME with your GitHub handle)
git remote add origin https://github.com/YOUR_USERNAME/metaog-studio.git

# Push to GitHub
git push -u origin main
```

#### Step 3: Enable Automated GitHub Pages Deployment
1. Go to your repository **Settings** > **Pages** (on the left menu).
2. Under **Build and deployment** > **Source**:
   * Select **GitHub Actions** (the included `.github/workflows/deploy.yml` will automatically deploy on every push).
   * *Alternatively*, choose **Deploy from a branch** > select `main` > root `/(root)` > click **Save**.
3. In under 60 seconds, your application will be live at:
   ```
   https://YOUR_USERNAME.github.io/metaog-studio/
   ```

---

## 📁 Repository Structure

```text
├── .github/
│   └── workflows/
│       └── deploy.yml      # Automated GitHub Pages CI/CD workflow
├── .gitignore              # Ignores OS/editor temporary files
├── index.html              # Complete single-file application (UI, SVG engine, scraper)
├── LICENSE                 # Open-source MIT License
├── package.json            # Project metadata and quick preview scripts
├── README.md               # Project documentation and deployment guide
└── robots.txt              # Search engine crawler instructions
```

---

## 🛠️ Technology Stack

* **Core**: HTML5, Vanilla JavaScript (ES6+), Canvas API.
* **Styling**: Tailwind CSS via CDN.
* **Icons**: [Lucide Icons](https://lucide.dev/).
* **Typography**: Google Fonts (*Plus Jakarta Sans*, *Inter*, *Outfit*, *Space Grotesk*, *Poppins*, *Playfair Display*, *Roboto Mono*, *JetBrains Mono*).

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.