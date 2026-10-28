# Engineering Notes

A small, static personal notes site intended for GitHub Pages. The homepage is `index.html`; individual notes live in subject folders under `notes/`.

## Preview locally

Open `index.html` in a browser, or run this from the project folder:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`. The System Design Notebook uses Google Fonts and Mermaid from CDNs, so those enhancements need an internet connection.

## Add a note

1. Create a subject folder such as `notes/databases/`.
2. Put your HTML note inside it, for example `notes/databases/indexes.html`.
3. Add a card to `index.html` with a relative link such as `notes/databases/indexes.html`.

Keep links relative (do not start them with `/`) so they work locally and under a GitHub repository subpath.

## Publish with GitHub Pages

1. Create a GitHub repository and push this project to its `main` branch.
2. On GitHub, open **Settings** → **Pages**.
3. Select **Deploy from a branch**.
4. Choose **main** and **/(root)**, then save.
5. GitHub will show your public URL. Future pushes to `main` update the site.

The URL is normally `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`. All links are relative, so no changes are needed for that repository subpath.
