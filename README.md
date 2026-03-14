# Personal Academic Website

This is a personal academic website built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

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
└── docs/                # Generated website (auto-created)
```

## Setup Instructions

### 1. Install Quarto

Download and install Quarto from: https://quarto.org/docs/get-started/

### 2. Customize Your Content

Edit the following files with your actual information:

- **`_quarto.yml`**: Update the website title with your name
- **`index.qmd`**: Fill in your bio, education, research experience, and skills
- **`publications.qmd`**: Add your publications
- **`projects.qmd`**: Describe your research projects
- **`contact.qmd`**: Add your contact information and links

### 3. Add Your Photo (Optional)

Place your profile photo in the `images/` folder and update `index.qmd`:

```markdown
<center>
<img src="images/profile.jpg" alt="Your Name" class="roundedimg" width="200px"/>
</center>
```

### 4. Build the Website

Run the following command in the terminal:

```bash
quarto render
```

This will generate the website in the `docs/` folder.

### 5. Deploy to GitHub Pages

1. Push all files to your GitHub repository
2. Go to repository Settings → Pages
3. Set Source to "Deploy from a branch"
4. Select "main" branch and "/docs" folder
5. Click Save

Your website will be available at: `https://siyuchen1111.github.io`

## Updating Your Website

To update content:
1. Edit the relevant `.qmd` files
2. Run `quarto render` to rebuild
3. Push changes to GitHub

## Customization

### Changing Colors

Edit `styles.css` to modify the sidebar color or other styles:

```css
.sidebar.sidebar-navigation {
  background-color: #668ABE !important;  /* Change this color */
}
```

### Adding New Pages

1. Create a new `.qmd` file
2. Add it to `_quarto.yml` in the sidebar contents section

## References

This website is based on the structure of [poldracklab.github.io](https://poldracklab.github.io).

## License

[Add your preferred license]
