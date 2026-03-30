# Babyshop Engine

Static deploy-ready prompt generator for Babyshop workflows.

## Repo structure

```text
babyshop-engine-repo/
├── index.html
├── .gitignore
├── .nojekyll
├── README.md
└── assets/
    ├── css/
    │   └── styles.css
    ├── js/
    │   └── app.js
    └── data/
        └── babyshop_base_prompts.csv
```

## What is included

- Updated Babyshop prompt engine
- Split frontend files for cleaner GitHub deployment
- Import / export resource workflow
- Base prompts bundled in the app
- CSV source file included for reference

## Deploy on GitHub Pages

1. Create a new GitHub repository.
2. Upload all files from this folder to the root of the repo.
3. Make sure the main app file is named `index.html`.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / `(root)`
6. Save, then wait for GitHub Pages to publish.

## Local preview

Open `index.html` directly in a browser, or serve it locally with a static server.

Example:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Notes

- App state is stored in browser local storage.
- Importing new resources updates the in-browser library instantly.
- Reset options restore built-in data for the selected resource type.
