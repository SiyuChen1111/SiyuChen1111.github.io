# Personal Academic Website

This is a personal academic website built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

**Website URL:** https://siyuchen1111.github.io

## Website Structure

```
.
├── _quarto.yml          # Website configuration (navigation, theme)
├── styles.css           # Custom CSS styles (#668ABE sidebar)
├── index.qmd            # Home / About Me page
├── publications.qmd     # Publications list
├── projects.qmd         # Research projects
├── contact.qmd          # Contact information
├── images/              # Profile photos and other images
├── files/               # CV and other documents
│   └── CV_SiyuChen_v3.pdf
└── .github/
    └── workflows/
        └── publish.yml  # GitHub Actions for auto-deployment
```

## 🚀 Auto-Deployment (GitHub Actions)

This website is automatically built and deployed using GitHub Actions. Every time you push changes to the `main` branch, the website will be automatically rebuilt and updated.

### How it works:
1. You edit the `.qmd` files locally
2. Push changes to GitHub: `git push origin main`
3. GitHub Actions automatically:
   - Sets up Quarto
   - Renders the website
   - Deploys to GitHub Pages

## 📝 Updating Your Website

### Step 1: Edit Content
Edit the relevant `.qmd` files with your updates:
- `index.qmd` - Home page / About Me
- `publications.qmd` - Publications
- `projects.qmd` - Research projects
- `contact.qmd` - Contact information

### Step 2: Push to GitHub
```bash
git add .
git commit -m "Update website content"
git push origin main
```

### Step 3: Wait for Deployment
- Go to https://github.com/SiyuChen1111/SiyuChen1111.github.io/actions
- Watch the workflow run (takes ~2-3 minutes)
- Your website will be updated automatically!

## 🛠️ Manual Build (Optional)

If you want to build locally:

### 1. Install Quarto
Download from: https://quarto.org/docs/get-started/

### 2. Build the Website
```bash
quarto render
```

### 3. Preview Locally
```bash
quarto preview
```

## 📋 Important Notes

### CV File
Make sure to upload your CV to the `files/` folder:
```bash
cp /path/to/CV_SiyuChen_v3.pdf files/
git add files/
git commit -m "Add CV"
git push origin main
```

### Profile Photo (Optional)
To add a profile photo:
1. Place your photo in `images/profile.jpg` (or .png)
2. Uncomment the photo section in `index.qmd`

### Customization
Edit `styles.css` to change colors or styles:
```css
.sidebar.sidebar-navigation {
  background-color: #668ABE !important;  /* Change sidebar color */
}
```

## 🔧 GitHub Pages Settings

The website uses GitHub Actions for deployment. Make sure your repository settings are:

1. Go to Settings → Pages
2. Source: "GitHub Actions"
3. (Not "Deploy from a branch" - we use Actions instead)

## 📚 References

This website is based on the structure of [poldracklab.github.io](https://poldracklab.github.io).

## 📄 License

[Add your preferred license]
