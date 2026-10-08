# Dariya Group website

A scroll-driven site for Dariya Events, Dariya Gourmet, Qafila, Raviya Productions and Khanabadosh, with a dashboard at `/admin` for uploading photos, adding YouTube films and editing text.

## What's in the folder

| Path | What it is |
|---|---|
| `index.html` | The website |
| `content/*.json` | All text, houses, photos and films. The dashboard edits these. |
| `images/uploads/` | Where photos uploaded from the dashboard are stored |
| `admin/` | The dashboard (Decap CMS) |
| `src/page.html` | Design source. Only needed if a developer changes the layout. |

## Go live (free, about 20 minutes, one time)

1. **GitHub** — create a free account, then a new repository called `dariya-website`. Upload everything in this folder to it (Add file → Upload files → drag the whole folder contents).
2. **Dashboard address** — already set to `dariyaevents/dariya-website`. Nothing to edit.
3. **Netlify** — sign up at netlify.com with your GitHub account → *Add new site* → *Import from GitHub* → pick `dariya-website` → Deploy. No build settings needed.
4. **Let the dashboard log in** — on GitHub: Settings → Developer settings → OAuth Apps → New OAuth App.
   - Homepage URL: your Netlify site URL
   - Authorization callback URL: `https://api.netlify.com/auth/done`
   Copy the Client ID and generate a Client Secret. Then in Netlify: Site configuration → Access & security → OAuth → Install provider → GitHub → paste both.
5. **Domain** — Netlify → Domain management → add `dariyaevents.com` (or whichever you own) and follow the DNS steps. HTTPS is automatic. Update `site_url` in `admin/config.yml` to match.
6. **Enquiry form** — Netlify detects the form automatically. Enquiries appear under Netlify → Forms; turn on email notifications there so each one reaches your inbox.

## Using the dashboard

Go to `yoursite.com/admin`, log in with GitHub.

- **Photo gallery** — add a photo, choose the house, write a caption, pick Normal / Tall / Wide. Drag to reorder.
- **Films** — paste any YouTube link (watch, youtu.be or Shorts).
- **The five houses** — edit descriptions, services, accent colour, cover photo, FSSAI licence number.
- **Text, contact, FAQ & testimonials** — phone, WhatsApp, email, Instagram, FAQ answers. Testimonials stay hidden until you add a real one.

Click **Publish**. The live site updates in about a minute.

Photo tip: export JPGs around 2000px on the long side and under 600 KB. Large camera files will slow the site down.

## Before launch, check

- Phone number (currently a placeholder), email, WhatsApp, Instagram
- FAQ answers match how you actually work
- Replace the sample "Photo slot" and "Film slot" entries with real work, or delete them
