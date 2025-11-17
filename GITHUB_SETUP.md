# GitHub Upload & Shopify Integration Guide

## 📤 Step 1: Push Theme to GitHub

### Create a New GitHub Repository

1. Go to [GitHub.com](https://github.com/new)
2. Fill in repository details:
   - **Repository name:** `prakriti-essentials-shopify-theme`
   - **Description:** `Modern Shopify 2.0 theme for Prakriti Essentials natural wellness products`
   - **Visibility:** Public (or Private if preferred)
   - **Initialize with:** Add .gitignore (already done locally)
3. Click **Create repository**

### Push Your Local Files to GitHub

Open PowerShell and run these commands in the theme directory:

```powershell
cd c:\Users\PC\Downloads\prakiriti

# Initialize git (if not already initialized)
git init

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR-USERNAME/prakriti-essentials-shopify-theme.git

# Rename branch to main (if needed)
git branch -M main

# Stage all files
git add .

# Create initial commit
git commit -m "Initial commit: Complete Shopify 2.0 theme for Prakriti Essentials"

# Push to GitHub
git push -u origin main
```

Replace `YOUR-USERNAME` with your actual GitHub username.

---

## 🔌 Step 2: Connect GitHub to Shopify Admin

### Option A: Using Shopify CLI (Recommended)

1. **Install Shopify CLI** (if not installed):
   ```powershell
   npm install -g @shopify/cli @shopify/theme
   ```

2. **Navigate to your theme directory:**
   ```powershell
   cd c:\Users\PC\Downloads\prakiriti
   ```

3. **Login to Shopify:**
   ```powershell
   shopify theme dev
   ```
   - This will open a browser to authenticate
   - Select your store
   - You'll get a preview URL

4. **Push theme to Shopify:**
   ```powershell
   shopify theme push --unpublished
   ```
   - Creates unpublished theme from GitHub repo
   - You can then publish it in Shopify Admin

### Option B: Manual Upload (If GitHub Connection Unavailable)

1. Go to **Shopify Admin** → **Online Store** → **Themes**
2. Click **Upload theme**
3. Upload the `prakriti-essentials-shopify-theme.zip` (0.95 MB)
4. Click **Upload**

---

## 📁 GitHub Repository Structure

Your repository should look like this:

```
prakriti-essentials-shopify-theme/
├── README.md                    # Documentation
├── theme.toml                   # Theme metadata
├── .gitignore                   # Git ignore rules
├── assets/                      # CSS, JS, SVG assets (200+ files)
├── config/                      # Theme settings
│   ├── settings_data.json       # Pre-configured settings
│   └── settings_schema.json     # Customization options
├── layout/                      # Theme layouts
│   ├── theme.liquid
│   └── password.liquid
├── locales/                     # Multi-language translations (45+ files)
├── sections/                    # Liquid section files (45+ files)
├── snippets/                    # Reusable snippets (35+ files)
└── templates/                   # JSON templates (23 files)
    ├── index.json               # Homepage
    ├── product.json             # Product page
    ├── collection.json          # Collection page
    ├── cart.json                # Cart page
    ├── page.faq.json            # FAQ page
    └── ... (18 more templates)
```

**Total:** 500+ files across all directories

---

## ✅ Verification Checklist

- [ ] Repository created on GitHub
- [ ] Local files pushed to GitHub (`git push`)
- [ ] Shopify CLI installed (`shopify theme dev` works)
- [ ] Authenticated with Shopify (`shopify login`)
- [ ] Theme uploaded to Shopify (`shopify theme push`)
- [ ] Theme appears in Shopify Admin > Themes
- [ ] No 404 errors in browser console
- [ ] CSS and JS files loading properly
- [ ] Homepage displays correctly
- [ ] All sections accessible in theme editor

---

## 🔄 Updating Theme After Changes

After making changes locally:

```powershell
# Stage changes
git add .

# Commit changes
git commit -m "Update theme: [describe your changes]"

# Push to GitHub
git push origin main

# Push to Shopify (if using CLI)
shopify theme push
```

---

## 🆘 Troubleshooting

### "Refused to apply style" errors
- **Cause:** Incomplete theme zip (missing assets, layout, sections)
- **Solution:** Ensure all folders are included (✅ Already done in new zip)

### GitHub push fails
- **Cause:** Remote URL incorrect or authentication issue
- **Solution:** 
  ```powershell
  git remote -v  # Check current remote
  git remote set-url origin https://github.com/YOUR-USERNAME/repo-name.git
  ```

### Shopify CLI authentication fails
- **Cause:** Not logged in to Shopify
- **Solution:**
  ```powershell
  shopify login --shop your-store.myshopify.com
  ```

### Theme not appearing after push
- **Cause:** May need to publish in Shopify Admin
- **Solution:**
  1. Go to **Shopify Admin** → **Online Store** → **Themes**
  2. Find the unpublished theme
  3. Click **...** → **Publish**

---

## 📝 Commit Message Examples

```
Initial commit: Complete Shopify 2.0 theme for Prakriti Essentials

Update theme colors to match brand guidelines

Add FAQ page template with expandable accordions

Fix cart drawer styling and animations

Update product page with new review section
```

---

## 🔐 Important Notes

- **Do NOT commit:**
  - `.env` files with API keys
  - `node_modules/` directory
  - Temporary files (`*.zip`, preview.html)
  - `.DS_Store` or `Thumbs.db`

- **Always commit:**
  - `config/` (settings)
  - `templates/` (all JSON)
  - `assets/` (CSS, JS, SVG)
  - `sections/` (Liquid files)
  - `README.md` and `theme.toml`

---

## 🎯 Next Steps

1. ✅ Create GitHub repository
2. ✅ Push theme files to GitHub
3. ✅ Install Shopify CLI (if not done)
4. ✅ Authenticate with Shopify
5. ✅ Push theme to Shopify store
6. ✅ Verify in Shopify Admin
7. ✅ Create required collections
8. ✅ Add products with images
9. ✅ Publish theme to live store

---

## 📞 Support Resources

- [Shopify Theme Development](https://shopify.dev/themes)
- [Shopify CLI Documentation](https://shopify.dev/themes/tools/cli/getting-started)
- [GitHub Documentation](https://docs.github.com/en/repositories)
- [Shopify Community Forums](https://community.shopify.com)

---

**Theme Version:** 1.0.0  
**Updated:** November 17, 2025  
**Status:** Ready for GitHub & Shopify Deployment ✅
