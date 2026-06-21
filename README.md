# Soul Line — Website

The official website for *Soul Line* by Salena Bell.

## Structure

```
soulline-repo/
├── index.html              ← Main site (single-file: HTML/CSS/JS)
├── netlify.toml             ← Netlify build & routing config
├── assets/
│   └── images/              ← Book cover, photos, etc. go here
└── netlify/
    └── functions/           ← Serverless functions (future: quiz scoring, etc.)
```

## Local development

This is currently a static single-file site — no build step required.
Just open `index.html` in a browser, or use a local server:

```bash
npx serve .
```

## Deployment

Connected to Netlify. Every push to `main` auto-deploys.

## Forms

Four forms are wired up via [Netlify Forms](https://docs.netlify.com/forms/setup/):
- `reader-circle` — community signup
- `get-the-book` — book purchase link request
- `assessment-waitlist` — soul line assessment waitlist
- `contact` — general contact form

Submissions appear in your Netlify dashboard under **Forms**.
Set up email notifications: Site settings → Forms → Form notifications.

## Roadmap

- [ ] Add real book cover image (replace placeholder SVG in `index.html`)
- [ ] Build Soul Line Assessment (quiz)
- [ ] Add Supabase for user profiles + saved quiz results
- [ ] Reader community chat (Discord embed → native chat later)
- [ ] Connect form notifications to email/Mailchimp
