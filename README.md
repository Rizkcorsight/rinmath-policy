# rinmath-policy

GitHub Pages site for the Rinmath privacy policy.

Live URL after deploy: <https://rizkcorsight.github.io/rinmath-policy/>

## Deploy steps

1. Create a new public repo on GitHub named `rinmath-policy`.
2. Upload the three files in this folder (`index.md`, `_config.yml`,
   `README.md`) to the root of that repo. Easiest path: GitHub web UI
   → "Add file → Upload files".
3. In the new repo, go to **Settings → Pages**.
4. Under "Build and deployment", set:
   - Source: **Deploy from a branch**
   - Branch: **main** / folder: **/ (root)**
5. Save. GitHub Pages will build the site within a minute or two and
   surface the live URL at the top of the Pages settings panel.
6. Use that URL in App Store Connect:
   - **App Privacy → Privacy Policy URL**
   - **General → App Information → Privacy Policy URL**

## Updating the policy later

Edit `index.md` directly in the GitHub web UI. Bump the
"Last updated" date at the top, commit. Pages rebuilds automatically.
The App Store Connect URL stays the same — Apple just fetches the
latest content from the URL the next time a reviewer opens it.

## Optional: custom domain

If you want `privacy.rinmath.app` instead of the github.io URL, add a
`CNAME` file at the repo root containing only `privacy.rinmath.app`,
then point that subdomain at GitHub Pages from your DNS provider per
[GitHub's docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
