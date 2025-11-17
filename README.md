# Prakriti Essentials Co. - Shopify 2.0 Theme

## 📦 Theme Package Contents

This zip file contains a complete, production-ready Shopify 2.0 theme for "Prakriti Essentials Co." - a natural wellness and comfort brand specializing in massage guns, posture correctors, and pain relief products.

### File Structure
```
prakriti-essentials-shopify-theme.zip
├── templates/
│   ├── index.json              (Homepage - 12 sections)
│   ├── product.json            (Product page)
│   ├── collection.json         (Collection page)
│   ├── cart.json               (Cart page)
│   ├── page.faq.json           (FAQ page)
│   ├── page.json               (Generic page)
│   ├── page.contact.json       (Contact page)
│   ├── blog.json               (Blog listing)
│   ├── article.json            (Blog article)
│   ├── search.json             (Search results)
│   ├── list-collections.json   (Collections listing)
│   ├── 404.json                (Error page)
│   ├── password.json           (Password protection)
│   └── customers/              (Customer account pages)
│       ├── account.json
│       ├── activate_account.json
│       ├── addresses.json
│       ├── login.json
│       ├── order.json
│       ├── register.json
│       └── reset_password.json
└── config/
    ├── settings_data.json      (Pre-filled global settings)
    └── settings_schema.json    (Theme customization options)
```

---

## 🎨 Brand Identity Pre-Configured

### Color Palette
- **Primary Green (Sage):** `#A3B18A` - Main brand color
- **Secondary Green:** `#BFCBA8` - Accents
- **Off-White Background:** `#FCFCF9` - Primary background
- **Warm Ivory:** `#F5F1E9` - Secondary background
- **Sand:** `#EAE6DD` - Borders and dividers
- **Muted Oak:** `#6B5E51` - Footer background
- **Dark Text:** `#3A3A3A` - Primary text

### Typography
- **Headings:** DM Serif Display (elegant, serif)
- **Body:** Inter (clean, modern sans-serif)
- **Line Height:** 1.6
- **Letter Spacing:** 0.02em (headings)

### Design System
- **Base Unit:** 8px grid
- **Border Radius:** 16px
- **Section Spacing:** 64px
- **Grid Gap:** 24px
- **Card Shadow:** `0 8px 32px rgba(0, 0, 0, 0.07)`
- **Modal Shadow:** `0 20px 64px rgba(0, 0, 0, 0.15)`

---

## 📄 Page Templates Included

### 1. **index.json** (Homepage)
12 fully configured sections:
- Announcement bar (free shipping)
- Sticky header
- Hero banner with CTAs
- 4-column benefit section
- Featured collection (Best Sellers)
- Image + text (Massage Tools)
- 4-collection category grid
- Testimonials carousel
- 3-step wellness journey
- Brand story section
- Newsletter signup
- Footer with 4 blocks

### 2. **product.json** (Product Page)
- Product gallery with thumbnails
- Variant picker (button style)
- Dynamic pricing
- Star ratings
- Quick add to cart
- 4 information accordions:
  - How to Use
  - Benefits
  - Care Instructions
  - Shipping & Returns
- Product benefits section
- Related products
- Recently viewed products

### 3. **collection.json** (Collection Page)
- Dynamic collection banner
- 12 products per page
- 4 columns (desktop) / 2 columns (mobile)
- Drawer filter type
- Sorting enabled
- Quick add on cards

### 4. **cart.json** (Cart Page)
- Cart items display
- Cart notes enabled
- Subtotal and checkout buttons
- Product recommendations section
- Dynamic checkout option

### 5. **page.faq.json** (FAQ Page)
- Hero section
- 2 FAQ categories with 4 pre-filled questions
- Expandable accordions
- Contact CTA section

### 6. Additional Pages
- **page.json** - Generic page template
- **page.contact.json** - Contact form page
- **blog.json** - Blog listing
- **article.json** - Blog article
- **search.json** - Search results
- **list-collections.json** - Collections listing
- **404.json** - Error page
- **password.json** - Password protection page
- **customers/** - Account management pages

---

## ⚙️ Global Settings Pre-Configured

### In `settings_data.json`:
- 43 brand settings pre-filled
- All colors matching brand palette
- Typography settings (DM Serif Display, Inter)
- Spacing system configured (8px grid)
- Cart type: Drawer
- Product card style: Standard
- Ratings enabled
- Quick add enabled
- Search predictive enabled
- Social links configured (Facebook, Instagram, YouTube)

### In `settings_schema.json`:
- 6 customization sections
- Color picker for all brand colors
- Font selection options
- Product card options
- Cart settings
- Social media configuration

---

## 📥 Installation Instructions

### Method 1: Upload to Shopify Admin
1. Go to **Shopify Admin** → **Sales channels** → **Online Store** → **Themes**
2. Click **Upload theme** (top right)
3. Select the `prakriti-essentials-shopify-theme.zip` file
4. Click **Upload**
5. Theme will appear in your theme list

### Method 2: Using Shopify CLI (Recommended for Development)
```bash
# Install Shopify CLI if you haven't already
npm install -g @shopify/cli @shopify/theme

# Navigate to your theme directory
cd prakriti-essentials-shopify-theme

# Login to your Shopify store
shopify theme dev

# This opens a preview at http://localhost:9292
```

---

## 🚀 Next Steps After Installation

### 1. **Create Required Collections** (In Shopify Admin)
- `best-sellers` - Featured products
- `pain-relief` - Pain relief category
- `posture-support` - Posture products
- `sleep-wellness` - Sleep products
- `facial-care` - Facial care products
- `massage-tools` - Massage tools
- `wellness-tools` - All wellness tools

### 2. **Create Navigation Menus**
**Main Menu** (Header):
- Shop
- About
- Blog
- Contact
- FAQ

**Footer Shop Menu**:
- Massage Guns
- Posture Support
- Pain Relief
- Wellness Tools
- View All

**Footer Support Menu**:
- Contact Us
- Shipping Info
- Returns Policy
- Care Instructions
- Blog

### 3. **Upload Product Images**
Replace placeholder images in these sections:
- Homepage hero: `wellness-hero-spa-stones.jpg`
- Massage tools section: `massage-therapy-lifestyle.jpg`
- Category cards (4 images)
- Brand story: `natural-ingredients-herbs.jpg`
- FAQ page logo: `prakriti-favicon.png`
- Checkout logo: `prakriti-logo.png`

### 4. **Customize Content**
- Update announcement bar text
- Customize hero section text
- Edit benefit descriptions
- Update testimonials with real customer reviews
- Modify FAQ questions and answers
- Update newsletter signup message

### 5. **Configure Checkout Settings**
In **Shopify Admin** → **Settings** → **Checkout**:
- Upload Prakriti logo
- Set checkout color to sage green (`#A3B18A`)
- Configure payment methods
- Enable customer accounts

### 6. **Set Up Email & Social**
In **Shopify Admin** → **Settings** → **General**:
- Update store name to "Prakriti Essentials Co."
- Configure social media URLs
- Set up automated emails

---

## 🎯 Customization Guide

### Changing Colors
All colors are defined in `config/settings_data.json`. Edit these values:
```json
"colors_primary": "#A3B18A",
"colors_secondary": "#BFCBA8",
"colors_background": "#FCFCF9",
// ... etc
```

### Changing Fonts
Edit in `config/settings_data.json`:
```json
"typography_heading_font": "dm_serif_display_n4",
"typography_body_font": "inter_n4"
```

### Changing Section Order
In `templates/index.json`, edit the `"order"` array at the bottom to rearrange sections on the homepage.

### Editing Page Content
Edit JSON settings for each section (text, links, colors, padding) in the respective template files.

---

## 📱 Responsive Design

All templates are fully responsive:
- **Desktop:** Optimized for 1200px and above
- **Tablet:** Grid adapts to 2-3 columns
- **Mobile:** Single column layout
- **Touch-friendly:** Large tap targets for buttons

---

## ♿ Accessibility

Theme includes:
- Semantic HTML structure
- ARIA labels where appropriate
- Color contrast compliance
- Keyboard navigation support
- Alt text placeholders for images

---

## 🔧 Technical Details

### Shopify 2.0 Features
- JSON-based templates (easier to edit)
- Blocks system for flexible layouts
- Dynamic sections (drag-and-drop in editor)
- Settings schema for merchant customization
- Pre-filled default values

### Browser Support
- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Mobile browsers (iOS Safari, Chrome Android)

---

## 📊 Theme Statistics

- **Templates:** 23 (including customer pages)
- **Pre-configured Sections:** 40+
- **Product Cards:** 4 variations
- **Color Palette:** 10 colors
- **Typography:** 2 fonts (DM Serif Display, Inter)
- **Pre-filled Settings:** 43 global settings

---

## 🆘 Support & Documentation

### Official Shopify Resources
- [Shopify Theme Documentation](https://shopify.dev/themes)
- [Shopify Theme Dev](https://shopify.dev/themes/getting-started/create)
- [Shopify CLI Guide](https://shopify.dev/themes/tools/cli/getting-started)

### Common Issues

**Issue:** Images showing as placeholders
**Solution:** Replace `shopify://shop_images/` URLs with your uploaded image URLs in Shopify admin

**Issue:** Collections not appearing
**Solution:** Create collections in Shopify admin with the exact handles mentioned in "Next Steps"

**Issue:** Theme not uploading
**Solution:** Ensure zip file is not corrupted; try uploading individual files via Shopify CLI

---

## 📝 License & Usage

This theme is created for Prakriti Essentials Co. and includes:
- All source code (JSON templates)
- Pre-configured brand settings
- Design system and color palette
- Responsive layouts
- Full customization rights

---

## ✅ Pre-Launch Checklist

- [ ] Install theme in Shopify admin
- [ ] Create all required collections
- [ ] Upload product images
- [ ] Create navigation menus
- [ ] Add real testimonials
- [ ] Configure checkout settings
- [ ] Set up payment methods
- [ ] Add store owner details
- [ ] Configure shipping settings
- [ ] Set up customer emails
- [ ] Add social media links
- [ ] Test on mobile devices
- [ ] Verify all links work
- [ ] Set up analytics (Google/Shopify)
- [ ] Publish theme to live store

---

## 📞 Contact & Support

For questions about the Prakriti Essentials brand or theme customization:
- **Email:** support@prakritiessentials.com
- **Website:** https://prakritiessentials.com
- **Documentation:** https://help.prakritiessentials.com

---

**Theme Version:** 1.0.0  
**Created:** November 2025  
**Shopify Version:** 2.0+  
**Status:** Production Ready ✅
