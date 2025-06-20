# Adrian's Blog

A personal blog built with Quarto and deployed on GitHub Pages.

## Setup Instructions

### 1. Repository Setup
- Make sure your repository is named `adrian-blog` (which it should be)
- The repository should be public for GitHub Pages to work

### 2. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section in the left sidebar
4. Under "Source", select "GitHub Actions"
5. This will use the workflow file in `.github/workflows/deploy.yml`

### 3. Local Development
To work on your blog locally:

```bash
# Install Quarto if you haven't already
# Visit: https://quarto.org/docs/get-started/

# Clone your repository
git clone https://github.com/YOUR_USERNAME/adrian-blog.git
cd adrian-blog

# Install dependencies
quarto install tinytex

# Preview your site locally
quarto preview
```

### 4. Adding Content
- Edit `index.qmd` for your homepage
- Edit `about.qmd` for your about page
- Add new `.qmd` files for blog posts
- Update `_quarto.yml` to add new pages to the navigation

### 5. Deployment
- Simply push your changes to the `main` branch
- GitHub Actions will automatically build and deploy your site
- Your site will be available at: `https://YOUR_USERNAME.github.io/adrian-blog`

## File Structure
- `_quarto.yml` - Main configuration file
- `index.qmd` - Homepage
- `about.qmd` - About page
- `styles.css` - Custom CSS styles
- `.github/workflows/deploy.yml` - GitHub Actions deployment workflow

## Customization
- Modify `_quarto.yml` to change themes, navigation, and other settings
- Edit `styles.css` to customize the appearance
- Add more pages by creating new `.qmd` files and updating the navigation in `_quarto.yml` 