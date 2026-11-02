# VMC's Life

A personal organizer in one static file: to-dos, projects, goals, habits, focus timer,
anti-procrastination helper, anti-brainrot detox, hobbies, money, wins timeline, vision board,
art games, mood and gratitude reflection, and a Self-Determination Theory check-in.

No build step. No server. Your data stays in your own browser (localStorage).

## Files
- `public/index.html`  the whole app
- `public/_headers`    security headers (Cloudflare reads this automatically)
- `wrangler.jsonc`     optional, for deploying with the Wrangler CLI

## Put it on GitHub
1. Create a new repository on github.com (private is fine).
2. Click "Add file" > "Upload files", drag in everything from this folder
   (keep the `public` folder), then "Commit changes".

## Deploy on Cloudflare Pages (connects to GitHub, auto-updates on every commit)
1. Cloudflare dashboard > Workers & Pages > Create > Pages > Connect to Git.
2. Pick your repository.
3. Framework preset: None. Build command: leave empty. Build output directory: `public`.
4. Save and Deploy. You get a `https://<name>.pages.dev` address.
5. Optional: Custom domains tab to use your own domain.
6. Optional privacy: Zero Trust > Access > Applications, to require a login before anyone can open it.

### Alternative: Wrangler CLI
    npm i -g wrangler
    wrangler login
    wrangler deploy

## On your Samsung phone
Open the address in Chrome, tap the three dots > "Add to Home screen".

## Good to know
- Data is saved per browser and per address. Use Home > Backup to copy your data code and
  restore it on another device.
- Keep the address the same. A new domain starts with empty data.
- Fonts load from Google Fonts. Everything else is self-contained.
