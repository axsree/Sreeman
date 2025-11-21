```markdown
# AXSREE — Static Website (Free deploy on GitHub Pages)

This repo contains a simple static site for AXSREE (HTML/CSS/JS). Designed to be deployed for free on GitHub Pages at the root domain:
https://axsree.github.io when the repository is named axsree.github.io (your GitHub username is axsree).

Files included:
- index.html
- styles.css
- script.js
- products.json
- assets/ (put your logo and images here)

Steps to finish and deploy

1) Add your images
   - Create an `assets/` folder and add:
     - `assets/logo.png` (save the logo you uploaded here as this filename)
     - `assets/product1.jpg`, `assets/product2.jpg`, `assets/product3.jpg` (replace with your photos)

2) Update WhatsApp number
   - Open `script.js` and replace the placeholder `phone` value ('919999999999') with your phone number (country code + number, e.g. 919876543210). This will be used for the "Order via WhatsApp" link.

3) Edit product info
   - Update `products.json` to add/remove products and point `image` to correct asset paths.

4) Create the GitHub repo (recommended repo name = axsree.github.io)
   - Create a new repository on GitHub named `axsree.github.io` (owner: axsree).
   - If the repo name matches that pattern, GitHub will serve the site at https://axsree.github.io automatically.

5) Push files from your machine (example commands)
   - In your project folder run:
     - git init
     - git add .
     - git commit -m "Initial AXSREE site"
     - git branch -M main
     - git remote add origin https://github.com/axsree/axsree.github.io.git
     - git push -u origin main

   (Or use SSH remote if you prefer: git@github.com:axsree/axsree.github.io.git)

6) After push
   - If the repo is named `axsree.github.io`, the site is usually live within a few minutes at:
     - https://axsree.github.io
   - If you use another repo name, enable GitHub Pages in repo Settings -> Pages and choose branch main / root.

Optional
- Use Netlify or Vercel instead if you prefer their deployment flow; both offer free plans and will work with this static site.
- Replace colors in `styles.css` (`:root` variables) to tweak brand look.
- Add a simple contact form via Formspree or getform if you want email submissions without a server.

If you want, I can:
- Provide the exact git commands again.
- Update the HTML to use an SVG logo filename if you upload an SVG file here.
- Help customize copy, add more products, or add a size selector and inventory note.

```