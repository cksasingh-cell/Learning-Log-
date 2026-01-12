# Deployment Guide

This guide will help you deploy Learning-Log to GitHub Pages.

## Quick Deployment (5 minutes)

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **+** icon in the top right
3. Select **"New repository"**
4. Name it `learning-log` (or any name you prefer)
5. Add description: "Personal knowledge companion for book notes"
6. Choose **Public** (required for free GitHub Pages)
7. Don't initialize with README (we already have one)
8. Click **"Create repository"**

### Step 2: Upload Files

#### Option A: Using GitHub Web Interface (Easiest)

1. In your new repository, click **"uploading an existing file"**
2. Drag and drop these files:
   - `index.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
   - `CONTRIBUTING.md`
3. Add commit message: "Initial commit"
4. Click **"Commit changes"**

#### Option B: Using Git Command Line

```bash
# Navigate to your project folder
cd /path/to/learning-log-github

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Learning-Log v1.0"

# Add remote repository (replace 'yourusername' with your GitHub username)
git remote add origin https://github.com/yourusername/learning-log.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Click **"Pages"** (left sidebar)
4. Under **"Source"**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **"Save"**
6. Wait 1-2 minutes for deployment

### Step 4: Access Your App

Your app will be live at:
```
https://yourusername.github.io/learning-log/
```

Replace `yourusername` with your actual GitHub username.

## Custom Domain (Optional)

If you want to use your own domain (e.g., `learninglog.com`):

1. Buy a domain from any registrar (GoDaddy, Namecheap, etc.)
2. In your repository Settings → Pages
3. Enter your custom domain
4. In your domain registrar, add DNS records:
   ```
   Type: A
   Host: @
   Value: 185.199.108.153
   
   Type: A
   Host: @
   Value: 185.199.109.153
   
   Type: A
   Host: @
   Value: 185.199.110.153
   
   Type: A
   Host: @
   Value: 185.199.111.153
   
   Type: CNAME
   Host: www
   Value: yourusername.github.io
   ```
5. Wait for DNS propagation (can take 24-48 hours)

## Updating Your Deployment

When you make changes to the app:

### Using Git:
```bash
# Make your changes to files

# Stage changes
git add .

# Commit changes
git commit -m "Description of changes"

# Push to GitHub
git push origin main
```

### Using GitHub Web Interface:
1. Go to the file on GitHub
2. Click the pencil icon (Edit)
3. Make your changes
4. Click "Commit changes"

GitHub Pages will automatically update within 1-2 minutes.

## Troubleshooting

### App not loading
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages for deployment status
- Make sure `index.html` is in the root directory
- Clear browser cache and try again

### 404 Error
- Verify the repository is public
- Check that Pages is enabled in Settings
- Ensure branch is set to `main` and folder to `/ (root)`

### Changes not appearing
- Wait 1-2 minutes for deployment
- Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)
- Check GitHub Actions tab for build status

## Build Status

GitHub Pages builds are automatic. Check status at:
```
https://github.com/yourusername/learning-log/actions
```

## Security & Privacy

- All data is stored locally in users' browsers
- No data is sent to any server
- GitHub Pages only hosts the static files
- Users' notes are private and never leave their device

## Performance

GitHub Pages provides:
- Free HTTPS
- Global CDN
- Fast loading times
- 99.9% uptime

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Open an Issue](https://github.com/yourusername/learning-log/issues)
- Check existing issues for solutions

---

**Congratulations!** Your Learning-Log is now live and accessible to everyone! 🎉
