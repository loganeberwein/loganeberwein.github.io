# Crawlable professional-profile website

This starter site is adapted from the LinkedIn PDF provided in chat. It deliberately excludes the email address, exact school, and grade/year details. Review all text before making it public.

## Publish on GitHub Pages

1. Log in to GitHub as `loganeberwein6`.
2. Create a **public** repository named **`loganeberwein6.github.io`** (if that repository does not already exist). If it already exists, add the files to it instead of making a new repository.
3. Upload every file from this folder into the repository root, including the blank `.nojekyll` file.
4. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select **main** and **/(root)**, then save.
5. Once the site is deployed, check `https://loganeberwein6.github.io/` in an incognito browser and verify that `https://loganeberwein6.github.io/robots.txt` and `/sitemap.xml` are visible without signing in.
6. Add the site URL to LinkedIn's contact info, GitHub profile, and ORCID record if desired.

## Submit for search indexing

- Google Search Console: https://search.google.com/search-console/ — add a URL-prefix property for `https://loganeberwein6.github.io/`, verify ownership using the provided HTML file option, use URL Inspection → Request indexing, and submit `sitemap.xml`.
- Bing Webmaster Tools: https://www.bing.com/webmasters/ — add and verify the site and submit the sitemap or URL.

You cannot force Google, Bing, or AI services to index, quote, or rank any site. In particular, you cannot force crawlers to get past LinkedIn's authentication wall. This website serves as an accessible alternative.

## AI crawler permissions

The included `robots.txt` allows OAI-SearchBot (ChatGPT search) and GPTBot (potential use in model training). These are separate purposes; you can disallow GPTBot and leave OAI-SearchBot allowed if you only want search discoverability. See official bot details at https://developers.openai.com/api/docs/bots . The optional `llms.txt` file is supplementary and is not guaranteed to be used by AI services.

## Using a different hostname

Before deploying on another domain, update all occurrences of `https://loganeberwein6.github.io/` in `index.html`, `robots.txt`, `sitemap.xml`, and `llms.txt` with the new site address.
