# itsbobbyswrld.com

Phase 1 production site for Bobby's WRLD LLC — the compliance/brand website
that backs the Apple Developer business URL, Twilio A2P 10DLC policy URLs,
and points to the Bobby's WRLD YouTube channel.

## Stack

- Plain semantic HTML + CSS (no JavaScript framework, no build step)
- Hosted on Vercel (static deploy, clean URLs by default)
- DNS via Cloudflare
- Email via Cloudflare Email Routing → forwards `hello@itsbobbyswrld.com`

## Deploy

`git push origin main` — Vercel auto-deploys from the main branch.

## Local preview

```
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

(On Windows: `python -m http.server 8000`.)

## File structure

```
itsbobbyswrld-com/
├── index.html              # Hero / ticker / about / footer
├── style.css               # Shared stylesheet for all pages
├── privacy/index.html      # Privacy Policy (Termly text pasted in later)
├── terms/index.html        # Terms of Service (Termly text pasted in later)
├── assets/
│   ├── logo-transparent.png
│   ├── favicon.ico
│   ├── favicon-16.png
│   ├── favicon-32.png
│   └── favicon-180.png
└── README.md
```

## TODO before launch

- Paste Termly-generated Privacy Policy into `privacy/index.html`.
- Paste Termly-generated Terms of Service into `terms/index.html`.
- Set the `Effective:` date on both legal pages.
