# MAHIDI Web Development

## Files
- `index.html`: bilingual English/Pashto website.
- `admin/`: Decap CMS admin interface and configuration.
- `content/homepage.json`: starter editable content.

## Important: publishing and admin activation
The public website can be deployed as a static site. The `/admin/` page is included, but it will NOT be able to save edits until the project is connected to a GitHub repository and authentication is configured.

1. Create a GitHub repository named `mahidi-web-development`.
2. Upload the contents of this folder (make sure `index.html` is in the repository root).
3. In `admin/config.yml`, replace `YOUR_GITHUB_USERNAME` with the real GitHub username.
4. Connect that repository to Netlify and deploy it.
5. In Netlify, configure the GitHub OAuth provider for Decap CMS (OAuth client credentials must be kept in Netlify settings, never put secrets in website files).
6. After auth is configured, open `https://YOUR-SITE.netlify.app/admin/` and sign in.

Netlify's legacy Git Gateway is deprecated for new setups, so this starter uses Decap's GitHub backend. The GitHub OAuth provider and repository permissions must be configured before admin publishing works.

## Visitor counter
The visitor display uses CounterAPI's public counter endpoint. It is an approximate public page-view counter, not secure analytics; public counters can be manipulated and the counter service may be unavailable at times. If it does not load, the site shows a dash rather than breaking the page.

## Contact privacy
The email, WhatsApp and Facebook links are visible to every visitor. Since this is a young person's public business site, get a parent/guardian's approval before publishing personal contact details. Consider using a separate business email and an adult-managed business contact number.

## Local preview
Open `index.html` in a browser. The visitor counter requires an internet connection. The admin login requires deployment and the authentication setup above.
