# Deployment Steps for EN Trade & Logistics LLC

## Option A — Fastest: Netlify drag-and-drop

1. Go to Netlify.
2. Open "Sites".
3. Drag the whole website folder into Netlify.
4. Netlify gives you a temporary URL.
5. Test the site.
6. Add your custom domain later.

## Option B — Better: GitHub + Netlify

1. Create GitHub repo:
   `en-trade-logistics-site`

2. Put these files inside the repo:
   - `index.html`
   - `styles.css`
   - `netlify.toml`

3. Push to GitHub.

4. In Netlify:
   - Add new site
   - Import from GitHub
   - Select repo
   - Build command: empty
   - Publish directory: `.`
   - Deploy

## Connect GoDaddy domain

In Netlify:
1. Site settings
2. Domain management
3. Add custom domain
4. Type your domain
5. Netlify will show DNS records

In GoDaddy:
1. Go to your domain
2. DNS
3. Add/change the records Netlify gives you

Usually it will be either:

- CNAME for `www`
- A records for root domain, or Netlify DNS nameservers

## Important

Do not cancel the domain itself at GoDaddy.
Only cancel GoDaddy website builder if you no longer want to use their layout builder.
