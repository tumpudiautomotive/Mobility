# Tumpudi Automotive website

Complete static website: HTML, CSS, JavaScript, images and PDF brochures. No build step, npm installation or API keys are required.

## Upload to GitHub

1. Extract this ZIP on your computer.
2. Create a GitHub repository, for example `tumpudi-automotive`.
3. Choose **Add file → Upload files**.
4. Upload the extracted files and the entire `assets` folder into the repository root. `index.html` must be at the root, not inside an extra folder. Upload the extracted contents, not the ZIP itself.
5. Commit the changes.

## Publish with GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Choose **main** and **/(root)**, then save.
4. GitHub will show the published website address after deployment.

The `.nojekyll` file is included. If your file picker hides it, the site still uses ordinary asset names; you can add the empty file separately if needed.

## Local preview

Open a terminal in the extracted folder and run:

```sh
python -m http.server 8000
```

Then open http://localhost:8000 in a browser. On Windows you may need `py -m http.server 8000`.

## Files

- `index.html`: Home and model chooser popup
- `models.html`: Models & Prices, charging/range and savings calculator
- `story.html`: Our Story
- `business.html`: Business
- `contact.html`: Contact
- `assets/`: Motorcycle and lifestyle images, logo and PDF brochures
- CSS and JavaScript files: Styling and interactions; keep all files provided

## Contact behaviour

Enquiry forms compose messages in WhatsApp. Visitors review and send the message there. The site does not store enquiries in a database. Telephone and email links use the visitor's installed apps.

## Editing

Page copy is in the HTML files. Model-specific values are in `product.js`. Savings calculations are in `savings-math.js`. Mobile hero styling is in `mobile-hero.css`; shared footer styling is in `footer.css`. Asset URLs are relative so the site works in a GitHub Pages project repository.

The package contains the latest approved mobile footer centring. Proposed engineering specifications remain labelled as targets.
