# Vidya Samiksha Kendra (VSK Bihar) - Live GitHub Ready Website

This directory contains the production-ready, clean, modular static website for **Vidya Samiksha Kendra (Government of Bihar)**.

- **No bulky base64 strings**: `index.html` is lightweight (~28 KB).
- **100% Control of Design**: All stylesheets are cleanly separated in `css/`.
- **100% Control of Assets**: All 25 images are organized and clearly named in `images/`.
- **Zero Configuration Required**: Uses relative paths, meaning it works immediately on **GitHub Pages**, **Vercel**, **Netlify**, or local preview.

---

## Folder Structure

```
├── index.html                   # Main webpage (lightweight, clean markup)
├── css/
│   ├── main.css                 # Base theme and framework styling
│   └── custom.css               # Modern glass cards, quick access portals, responsive layout
└── images/
    ├── bihar_logo.png           # Bihar Government / VSK logo
    ├── bihar_hero_banner.png    # Hero section banner
    ├── about_analytics_dashboard.png # High-quality About section analytics dashboard (1024x576)
    │
    │   # 4 Quick Access Portals
    ├── portal_teacher.png       # Teacher Management portal
    ├── portal_student.png       # Student Lifecycle portal
    ├── portal_school.png        # School Governance portal
    ├── portal_ai_assistant.png  # AI Education Assistant portal
    │
    │   # 12 Key Educational Modules
    ├── module_school_info.png
    ├── module_teacher_insights.png
    ├── module_pm_poshan.png
    ├── module_learning_perf.png
    ├── module_education_kpis.png
    ├── module_today_insights.png
    ├── module_geomap.png
    ├── module_reports.png
    ├── module_office_admin.png
    ├── module_teacher_dev.png
    ├── module_ai_assistant.png
    ├── module_student_engagement.png
    │
    │   # Government & Institutional Partners
    ├── partner_nic.png
    ├── partner_ncert.png
    ├── partner_iit.png
    ├── partner_diksha.png
    ├── partner_samagra.png
    └── footer_samagra_logo.png
```

---

## 1-Minute GitHub Pages Live Deployment

1. Create a new public repository on GitHub (e.g. `vsk-bihar`).
2. Upload or push all files from this folder (`index.html`, `css/`, `images/`) into the repository root:
   ```bash
   git init
   git add .
   git commit -m "Deploy VSK Bihar live portal"
   git branch -M main
   git remote add origin https://github.com/<YOUR_USERNAME>/vsk-bihar.git
   git push -u origin main
   ```
3. In your GitHub repository:
   - Go to **Settings** -> **Pages**.
   - Under **Build and deployment** -> **Source**, select **Deploy from a branch**.
   - Set Branch: `main`, Folder: `/ (root)`, and click **Save**.
4. In under 60 seconds, your site is live at:
   `https://<YOUR_USERNAME>.github.io/vsk-bihar/`

---

## Using GitHub as a CDN for Another Website

If you host these assets on your public GitHub repository and want to render them on any other external HTML page or CMS, you can reference them via jsDelivr CDN:

- **CSS**:
  ```html
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/<YOUR_USERNAME>/vsk-bihar@main/css/main.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/<YOUR_USERNAME>/vsk-bihar@main/css/custom.css">
  ```

- **Images**:
  ```html
  <img src="https://cdn.jsdelivr.net/gh/<YOUR_USERNAME>/vsk-bihar@main/images/bihar_logo.png">
  <img src="https://cdn.jsdelivr.net/gh/<YOUR_USERNAME>/vsk-bihar@main/images/about_analytics_dashboard.png">
  ```

Or simply add a single `<base>` tag in the `<head>` of your HTML:
```html
<base href="https://cdn.jsdelivr.net/gh/<YOUR_USERNAME>/vsk-bihar@main/">
```
