# Luis Espinosa Anke - Academic Website

A modern, eye-catching academic portfolio website with a distinctive blue and yellow theme.

## 🎨 Design Features

- **Bold Blue & Yellow Theme**: Professional navy/royal blue with vibrant yellow accents
- **Modern Typography**: Playfair Display for headings, Work Sans for body text
- **Smooth Animations**: Scroll-triggered reveals and smooth transitions
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Clean Structure**: Easy to navigate sections for publications, research, teaching, and service

## 📁 Files

- `index.html` - Main HTML structure
- `styles.css` - All styling with CSS variables for easy customization
- `script.js` - Interactive features and animations
- `profile.jpg` - Your profile photo

## 🚀 Deployment to GitHub Pages

### Step 1: Update Your GitHub Repository

1. Clone your repository (if you haven't already):
   ```bash
   git clone https://github.com/luisespinosaanke/luisespinosaanke.github.io.git
   cd luisespinosaanke.github.io
   ```

2. Copy all files from this folder to your repository:
   ```bash
   # Copy the files (adjust paths as needed)
   cp index.html styles.css script.js profile.jpg /path/to/luisespinosaanke.github.io/
   ```

3. Commit and push:
   ```bash
   git add .
   git commit -m "New academic website with blue/yellow theme"
   git push origin main
   ```

### Step 2: Configure Custom Domain in GitHub

1. Go to your repository settings: https://github.com/luisespinosaanke/luisespinosaanke.github.io/settings
2. Scroll to "Pages" section
3. Under "Custom domain", enter: `luisespinosa.net`
4. Save

### Step 3: Configure DNS in IONOS

You'll need to add these DNS records in your IONOS dashboard:

#### For APEX domain (luisespinosa.net):
Add these A records:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

#### For www subdomain:
Add a CNAME record:
```
www  →  luisespinosaanke.github.io
```

**Steps in IONOS:**
1. Log into IONOS
2. Go to Domains & SSL
3. Click on your domain (luisespinosa.net)
4. Go to DNS settings
5. Remove the current redirect
6. Add the A records and CNAME as shown above
7. Wait 24-48 hours for DNS propagation (usually faster, ~1-2 hours)

### Step 4: Enable HTTPS

1. Once DNS propagates, go back to GitHub Pages settings
2. Check "Enforce HTTPS" (may need to wait a bit for certificate generation)

## 🔧 Customization

### Update Content

To update your content, simply edit the `index.html` file:

- **Bio**: Search for the "about-text" section
- **Publications**: Update the "project-card" entries
- **Research Projects**: Modify the "research-card" sections
- **Teaching**: Edit the "course-card" elements
- **Service**: Update the "activity-list" items

### Change Colors

All colors are defined as CSS variables in `styles.css`. Look for the `:root` section:

```css
:root {
    --primary-blue: #0A2463;
    --accent-blue: #1E3A8A;
    --bright-yellow: #FFD700;
    /* ... etc */
}
```

### Add New Sections

Follow the existing section structure:

```html
<section id="new-section" class="section">
    <div class="container">
        <h2 class="section-title">Section Title</h2>
        <!-- Your content here -->
    </div>
</section>
```

## 📱 Mobile Responsive

The site is fully responsive and works beautifully on:
- Desktop (1920px+)
- Laptop (1024px - 1920px)
- Tablet (768px - 1024px)
- Mobile (320px - 768px)

## 🎯 Next Steps After Deployment

1. **Test the site** at luisespinosaanke.github.io
2. **Configure DNS** in IONOS (as described above)
3. **Wait for DNS propagation** (check with https://dnschecker.org/)
4. **Enable HTTPS** in GitHub settings
5. **Close your Jimdo site** once everything is working

## 📧 Need Help?

If you need to update content or make changes, the files are organized and commented for easy editing.

---

**Note**: The site uses Google Fonts (Playfair Display and Work Sans) which load from CDN. Make sure you have internet connectivity for fonts to display properly during development.
