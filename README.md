# Logan Eberwein — minimal profile website

A simple white, résumé-style version of the LinkedIn profile supplied as `Profile.pdf`. The wording in the Summary, Experience, Education, Publications, Top Skills and Languages sections is taken from the PDF, with only line breaks and layout adapted for the web.

## Photo

The upper-right corner has a portrait placeholder. To add your photo:

1. Put an image named `portrait.jpg` in the same folder as `index.html`.
2. In `index.html`, find the `photo-placeholder` div near the beginning of the `<main>` element.
3. Replace that div with:

   `<img class="portrait-image" src="portrait.jpg" alt="Portrait of Logan Eberwein">`

4. Optionally adjust the image cropping with the `.portrait-image` CSS class.

## Publish via GitHub Pages

1. Create or open the GitHub repository `loganeberwein6.github.io`.
2. Upload the contents of this folder, including `index.html`, `robots.txt`, `sitemap.xml`, `llms.txt` and `.nojekyll`, to the repository root.
3. Go to **Settings → Pages**, choose **Deploy from a branch**, then `main` and `/(root)`.
4. Once live, visit `https://loganeberwein6.github.io/` in an incognito window. Update `sitemap.xml`, `robots.txt` and the canonical URL if you use a different domain.

The site uses a few lines of JavaScript for subtle scroll-reveal animations and a thin reading-progress indicator. It respects reduced-motion settings. The text is rendered as normal HTML even without JavaScript, making it accessible to search engines and crawlers. It uses Google Fonts with local fallbacks.

## Privacy / accuracy check before publishing

This version **includes the email address, school, and grade/year details** from your uploaded LinkedIn PDF because you requested a near copy of it. You may wish to remove those details if you do not want them permanently discoverable by search engines and scrapers. Review the wording of the PDF for any outdated information before you publish.

Search engines and AI systems can be allowed to crawl a site, but indexing or citing it is never guaranteed.
