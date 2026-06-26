# DropOutsCore — GitHub Org Setup Guide

## What's in this folder

```
dropoutscore/
├── .github/
│   └── profile/
│       └── README.md     ← The ORG profile page (shown at github.com/DropOutsCore)
├── assets/
│   ├── banner.svg        ← Banner illustration  (1200 × 400)
│   └── logo.svg          ← Square logo mark     (200 × 200)
├── README.md             ← Shown when someone opens your .github repo
└── SETUP.md              ← This file (delete after setup)
```

---

## Upload steps

### 1 — Create the `.github` repo on GitHub
1. Go to **github.com/DropOutsCore** → New repository
2. Name it exactly: `.github`  ← the dot matters
3. Set visibility to **Public**
4. Skip the default README (you have your own)
5. Click **Create repository**

### 2 — Upload everything
Use **GitHub.com drag-and-drop** (easiest):
1. Open your new `.github` repo
2. Click **Add file → Upload files**
3. Drag the entire unzipped `dropoutscore/` folder contents in
4. Commit to `main`

Or push via git:
```bash
cd dropoutscore
git init
git remote add origin https://github.com/DropOutsCore/.github.git
git add .
git commit -m "feat: org profile and assets"
git push -u origin main
```

### 3 — Verify
Visit **github.com/DropOutsCore** — your org page should render with the banner, logo, and full README.

---

## Image URLs used in the profile README

The README at `.github/profile/README.md` uses these raw GitHub URLs:

```
https://raw.githubusercontent.com/DropOutsCore/.github/main/assets/banner.svg
https://raw.githubusercontent.com/DropOutsCore/.github/main/assets/logo.svg
```

These go live automatically once you push to the `main` branch of the `.github` repo.

---

## Customisation

- **Add socials**: replace the GitHub badge in the "Find Us" section with your LinkedIn / Twitter / portfolio links
- **Update stack**: edit the badge section as your stack evolves
- **Add projects later**: insert a table between the Philosophy and Tech Stack sections when ready
- **Edit SVGs**: both files open in Figma (File → Import), Inkscape, or any text editor

