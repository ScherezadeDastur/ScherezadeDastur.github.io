# Academic CV Website

A clean, elegant academic personal website — ready to host on GitHub Pages.

## Files

```
index.html       → Home page (bio, photo, contact)
research.html    → Publications & presentations
experience.html  → Teaching & academic experience
cv.html          → CV overview + download link
style.css        → All styles
main.js          → Mobile nav + scroll effects
cv.pdf           → ADD YOUR CV PDF HERE
photo.jpg        → ADD YOUR PHOTO HERE
```

## How to Customize

### 1. Replace placeholder text
Search for `Your Name`, `[Your Institution]`, `yourname@institution.edu`, etc. and replace with your real details across all `.html` files.

### 2. Add your photo
Put your photo (named `photo.jpg`, `photo.png`, or similar) in the same folder.

In `index.html`, replace this block:
```html
<div class="photo-placeholder">
  <span>Your Photo</span>
  <p class="photo-hint">Replace with &lt;img src="photo.jpg"&gt;</p>
</div>
```
with:
```html
<img src="photo.jpg" alt="Your Name" />
```

### 3. Add your CV PDF
Drop your CV as `cv.pdf` in the folder. The download button on `cv.html` already points to it.

### 4. Update navigation links (if you rename pages)
All 4 HTML files share the same `<nav>` — update all of them if you rename a page.

---

## Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `yourname.github.io` or any name).
2. Upload all files to the **root** of the repository (or a `docs/` folder).
3. Go to **Settings → Pages**.
4. Under "Source", select `Deploy from a branch`.
5. Choose `main` branch and `/ (root)` (or `/docs` if you used that folder).
6. Click **Save** — your site will be live at `https://yourusername.github.io/repo-name/`.

**Tip:** If you name your repo `yourusername.github.io`, the site will be at `https://yourusername.github.io/` directly.

---

## Color Customization

All colors are CSS variables in `style.css` at the top:

```css
:root {
  --bg:        #faf9f6;   /* page background */
  --accent:    #3d2e1e;   /* dark brown accent (buttons) */
  --accent2:   #7a5c3e;   /* lighter accent (year labels, links) */
  --link:      #4a3520;   /* link color */
  --link-hover:#b07040;   /* link hover */
}
```

Change these to match your preferences.
