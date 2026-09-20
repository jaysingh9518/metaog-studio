# 🔮 MetaOG Studio — OpenGraph & SEO Meta Tag Suite

A web application for designing social preview cards (1200×630 landscape & 1080×1080 square) and checking SEO meta tags in real-time.

---

## 🌟 Key Highlights

- **OpenGraph Graphic Studio**:
  - **Large Landscape** (1200 × 630 px) for Twitter large summary, Facebook, LinkedIn, Discord.
  - **Square Aspect Ratio** (1080 × 1080 px) for Instagram, Discord server previews, and mobile apps.
  - **Auto Color Extraction**: Upload any brand logo, and the studio samples dominant hues to synchronize the card background, badge, and typography.
  - **Export to High-Resolution PNG & Vector SVG**: Crisp output with 1-click clipboard integration.
- **SEO Meta Tag Inspector & Builder**:
  - Target **60 characters** for Meta Titles with real-time character meters.
  - Benchmark **131 characters** (optimal 120–160 range) for Meta Descriptions.
  - **Live Google SERP Simulator** (switch between Desktop and Mobile preview).
  - Automated SEO Health Score grading with audit checklist.
  - Generates HTML `<meta>` tags ready for production copy-pasting.
- **Modern UI/UX**:
  - Light mode as default with smooth Dark mode toggle.
  - Standalone single-file architecture with zero build step required.

---

## 🚀 Instant Deployment to GitHub Pages

### Step 1: Create a GitHub Repository
1. Navigate to [GitHub](https://github.com/new) and create a repository named `metaog-studio`.
2. Choose **Public**.

### Step 2: Push Local Files to GitHub
Open your terminal in the project directory:

```bash
# Initialize git
git init

# Add all files
git add .

# Commit changes
git commit -m "feat: initial commit of MetaOG studio app"

# Set main branch
git branch -M main

# Add remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/metaog-studio.git

# Push to GitHub
git push -u origin main
```

### Step 3: Enable GitHub Pages (Free Hosting)
1. In your GitHub repository, navigate to **Settings** > **Pages** (on the left sidebar).
2. Under **Build and deployment** > **Branch**:
   - Select `main`
   - Select folder `/(root)`
3. Click **Save**.
4. In about 60 seconds, your site will be live at:
   `https://YOUR_USERNAME.github.io/metaog-studio/`

---

## 🛠️ Tech Stack

- **HTML5 & Vanilla JavaScript**: Fast execution with zero dependencies.
- **Tailwind CSS**: Utility-first styling via CDN.
- **Lucide Icons**: Clean iconography.
- **HTML5 Canvas API**: Dominant color extraction and vector-to-raster image synthesis.

---

## 📄 License
MIT License. Feel free to use this in your commercial or personal projects!