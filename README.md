# BuildEasy — static legal & support pages

Plain HTML/CSS for **App Store** and **Google Play** listing URLs.

A workflow at [`.github/workflows/static.yml`](.github/workflows/static.yml) publishes the **repo root** to GitHub Pages via [GitHub Actions](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages). One-time setup: **Settings → Pages → Build and deployment → Source: GitHub Actions**. The workflow runs on pushes to **`main`** that touch `*.html`, `styles.css`, or the workflow file itself (or run it manually via **Actions → Deploy GitHub Pages → Run workflow**).

**Not legal advice.** Have counsel review legal text before you rely on it.

## Public contact

- **Support / privacy:** [buildeasyerp@gmail.com](mailto:buildeasyerp@gmail.com)

## Files

| File | Use in store consoles |
|------|------------------------|
| `privacy-policy.html` | **Privacy Policy URL** (Apple & Google) |
| `support.html` | **Support URL** (Apple; Google expects reachable support) |
| `terms-of-use.html` | Terms / EULA link if required or linked from the app |
| `account-deletion.html` | Link from privacy/support; align with Play account-deletion requirements |
| `index.html` | Optional hub; not required by stores |
| `styles.css` | Shared stylesheet (keep next to the HTML files) |

## Final URLs (examples)

If the Pages site is a **project site** (repo name e.g. `legal`):

- `https://YOUR_ORG.github.io/legal/privacy-policy.html`
- `https://YOUR_ORG.github.io/legal/support.html`

If you use an **organization user site** (repo name `YOUR_ORG.github.io`), paths are the same but without the repo segment if you place files at the root of that repo.

GitHub Pages may serve `privacy-policy.html` as `/privacy-policy` in some configurations; prefer the `.html` URL in store listings unless you add redirects.

Ensure the published policy matches what you declare in App Store Connect **App Privacy** and Google Play **Data safety**.
