# Adwait Hegde - Portfolio

Static personal website, ready for GitHub Pages. No build step or server is needed.

## Structure

```
index.html        Home page (About, Skills, Resume, Contact)
resume.html       Embedded PDF resume, with download links
404.html          Page GitHub Pages shows for unknown URLs
.nojekyll         Tells GitHub Pages to serve files as-is (no Jekyll processing)
assets/
  css/style.css   Site styles
  js/main.js      Typing animation, smooth scrolling, mobile nav, animations
  img/            Profile photo, hero background, favicons
  *.pdf           Resume and academic CV
  vendor/         Bootstrap, Boxicons, IcoFont, jQuery, Typed.js, AOS
```

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy to GitHub Pages

1. Push this folder to a GitHub repository.
   - Name it `adwait-hegde.github.io` to serve the site at `https://adwait-hegde.github.io/`.
   - Any other name serves it at `https://adwait-hegde.github.io/<repo-name>/`. In that case, change the
     "Back to Home" link in `404.html` to `/<repo-name>/`.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.

## Updating content

- Text: edit `index.html`.
- Profile photo: replace `assets/img/profile-img.jpg` (keep it square).
- Resume: replace `assets/Adwait_Hegde_Resume.pdf` or `assets/Adwait_Hegde_Academic_CV.pdf`.
- The contact form posts to Formspree (`https://formspree.io/f/xzbyowqg`).
