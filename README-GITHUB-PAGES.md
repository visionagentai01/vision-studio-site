# Publish VISION Studio with GitHub Pages

The web files below are safe to publish. They contain no TikTok key, token,
password or local configuration:

- `index.html`, `features.html`, `how-it-works.html`, `faq.html`,
  `about.html`, `support.html`, `privacy.html`, `terms.html`
- `styles.css`
- `favicon.ico`, `icon-32.png`, `icon-180.png`, `icon-192.png`,
  `icon-512.png`, `icon-1024.png`

`icon-1024.png` is the exact image to upload as the **App icon** in the TikTok
Developer Portal, so the favicon, the page headers and the app icon match.

1. Create a public GitHub repository named `vision-studio-site`.
2. Upload the web files listed above to the repository root. Do not upload
   this README or anything else from the VISION project.
3. Open **Settings → Pages** in the repository.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch **main**, folder **/(root)**, then press **Save**.
6. Wait for the green deployment confirmation.

The resulting URLs will be:

- `https://YOUR-GITHUB-USERNAME.github.io/vision-studio-site/`
- `https://YOUR-GITHUB-USERNAME.github.io/vision-studio-site/terms.html`
- `https://YOUR-GITHUB-USERNAME.github.io/vision-studio-site/privacy.html`
- `https://YOUR-GITHUB-USERNAME.github.io/vision-studio-site/support.html`

In the TikTok Developer Portal use the home URL as **Website URL**, and the
matching Terms and Privacy URLs in their dedicated fields. Keep
`ai_data/tiktok.json`, tokens, videos and the rest of VISION private.

GitHub Pages only hosts the public information and legal pages. VISION Studio
uses TikTok `FILE_UPLOAD` for videos, so video files do not need a public domain.
Public Direct Post still requires TikTok to approve the `video.publish` scope and
audit the API client. Keep `publishing_enabled` and `public_posting_approved`
false until that approval is complete.
