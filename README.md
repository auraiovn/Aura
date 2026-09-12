# AURA — GitHub Pages export

This package contains the latest saved AURA website, version 3, exported on 12 September 2026. The website code and local media match that saved version exactly.

## Files

| Location | Contents |
| --- | --- |
| `index.html` | Complete website: HTML, inline CSS and JavaScript |
| `assets/` | Three garment overlays, two reference photos and four MP4 videos |
| `.nojekyll` | Tells GitHub Pages to serve the static files directly |
| `README.md` | Publishing instructions |

No npm installation, build command, API key or application server is required for this prototype.

## Publish using the GitHub website

1. Unzip this package on your computer. Upload the extracted files, not the ZIP itself.
2. Create a public GitHub repository named `aura`, or use your intended repository.
3. Upload `index.html` and the complete `assets` folder to the repository root, preserving the folder structure. Upload the other included files too. `index.html` must be immediately visible in the repository, not inside another project folder. Commit the upload to `main`.
4. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**. Click **Save**.
5. When deployment completes, use **Visit site** on the Pages settings screen. For a repository named `aura`, the usual address is `https://YOUR-USERNAME.github.io/aura/`; replace the placeholder with your actual GitHub username.

Publishing instructions: [GitHub publishing source documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site). Entry-file and URL guidance: [Create a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Edit and preview

Edit `index.html` with a text editor. Styles are in the `<style>` section, page content is in `<main>`, and product data and interactions are in the final `<script>` section. Keep media paths relative to `index.html`.

For a local preview with Python installed, open a terminal in the extracted folder and run `python3 -m http.server 8000`, then visit `http://localhost:8000`.

## Current prototype behaviour

- Test Camera Live on the published HTTPS page or localhost and allow camera permission. Three outfits have transparent overlays; automatic alignment depends on the external MediaPipe helper. Manual adjustments and photo upload are included. Real-device camera operation has not been verified in this export task.
- Some photography, fonts and the pose helper still load from external services; the package is not fully offline.
- Checkout, sign-in, newsletter and enquiry forms demonstrate the interface. They do not process payments, send emails or submit to a production backend. Cart data is stored in the browser.

## Your custom domain

This export does not change DNS or connect `aura.io.vn` to GitHub. Publish and verify the GitHub Pages URL first. Connecting a custom domain is a separate step in GitHub Pages settings and at the domain's DNS provider; entering its name alone does not register or purchase it.
