# Sheet Music Reader

Static mobile practice site for piano sheet-music reading.

## Deploy

Use permanent static hosting, not a temporary tunnel:

- Cloudflare Pages: root directory `sheet-music-reader-site`, build command none, output directory `.`
- Netlify: connect the repo or drag this folder into Netlify Drop.
- Vercel: import this folder/repo as a static project.
- GitHub Pages: publish this folder with `index.html` at the site root.

No build step is required.

CLI path after Cloudflare auth:

```bash
npx --yes wrangler pages deploy . --project-name sheet-music-reader
```

Current permanent URL:

```text
https://sheet-music-reader.pages.dev/
```

## Run Locally

From this folder:

```bash
python3 -m http.server 8765
```

Open:

```text
http://127.0.0.1:8765/
```

Temporary `trycloudflare.com` links are for demos only and stop working when the tunnel process exits.
