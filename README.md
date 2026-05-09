# GT Racing Club — Website Template (English)

A fully featured Gran Turismo 7 racing club website template built on GitHub Pages. No server required.

## Quick Setup

1. Clone or fork this repository under your own GitHub account
2. Enable GitHub Pages: Settings → Pages → Branch: main / root
3. Edit `config.js` and set `REPO` to `your-username/your-repo-name`
4. Push — your site is live at `https://your-username.github.io/your-repo-name`

## Default Admin Credentials

- **Username:** `admin`
- **Password:** `admin123`

⚠️ Change these immediately in `admin.html` by replacing `ADMIN_USER` and `ADMIN_HASH`.

To generate a new password hash, open the browser console and run:
```js
crypto.subtle.digest('SHA-256', new TextEncoder().encode('yourpassword'))
  .then(b => console.log([...new Uint8Array(b)].map(x=>x.toString(16).padStart(2,'0')).join('')))
```

## Customisation

All club-facing text (name, tagline, welcome messages, copyright) is managed via **Admin → Manage Club**.

The logo can be updated via **Admin → Manage Club** — it updates across the entire site automatically.

## Structure

| File | Purpose |
|---|---|
| `config.js` | Repo name and branch — edit once on setup |
| `club-config.json` | Club texts and logo config |
| `calendario.json` | Championships data |
| `piloti_schede/` | Driver profile JSONs |
| `risultati/` | Race result files |
| `campionati/` | Championship pages |
| `trophy_png/` | Trophy images |

