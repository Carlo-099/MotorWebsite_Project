# Deployment Guide for GitHub Pages

This guide will help you deploy your Cafe Racer website to GitHub Pages without any errors or warnings.

## Prerequisites

- A GitHub account
- Git installed on your computer

## Step-by-Step Deployment

### 1. Create a New Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository (e.g., `cafe-racer-website`)
5. Make it **Public** (required for free GitHub Pages)
6. **Do NOT** initialize with README, .gitignore, or license
7. Click "Create repository"

### 2. Upload Your Files

#### Option A: Using GitHub Web Interface
1. In your new repository, click "uploading an existing file"
2. Drag and drop all your website files and folders
3. Add a commit message like "Initial website upload"
4. Click "Commit changes"

#### Option B: Using Git Commands
```bash
# Clone the repository (replace with your repository URL)
git clone https://github.com/yourusername/cafe-racer-website.git

# Copy all your website files to the repository folder
# (Make sure to include all HTML, CSS, and image files)

# Add all files to git
git add .

# Commit the changes
git commit -m "Initial website upload"

# Push to GitHub
git push origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section (in the left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select "main" and "/ (root)"
6. Click "Save"

### 4. Access Your Website

- Your website will be available at: `https://yourusername.github.io/cafe-racer-website`
- It may take a few minutes for the changes to appear
- You can check the deployment status in the "Actions" tab

## Important Notes

### HTTPS Ready
- ✅ All resources use relative paths
- ✅ No HTTP references found
- ✅ All links use `target="_self"` for consistency
- ✅ Mobile responsive design implemented

### File Structure
Make sure your repository contains:
```
cafe-racer-website/
├── index.html
├── about.html
├── contact.html
├── parts.html
├── helmet.html
├── example.html
├── README.md
├── .gitignore
├── Css/
│   ├── style.css
│   ├── about.css
│   ├── contact.css
│   ├── parts.css
│   ├── helmet.css
│   └── example.css
├── Motor.Picture/
├── Motor.parts/
└── Motor.helmet/
```

### Troubleshooting

**If you see a 404 error:**
- Make sure `index.html` is in the root directory
- Check that all file names match exactly (case-sensitive)

**If images don't load:**
- Verify all image files are uploaded
- Check that image paths in HTML files are correct

**If styles don't apply:**
- Ensure all CSS files are in the `Css/` folder
- Check that CSS file paths in HTML files are correct

## Custom Domain (Optional)

If you want to use a custom domain:
1. In repository Settings → Pages
2. Enter your domain in the "Custom domain" field
3. Add a CNAME file to your repository with your domain
4. Configure DNS settings with your domain provider

## Support

If you encounter any issues:
1. Check the "Actions" tab for deployment errors
2. Verify all files are properly uploaded
3. Test locally by opening `index.html` in a browser
4. Check browser console for any JavaScript errors

Your website is now ready for deployment on GitHub Pages! 🚀 