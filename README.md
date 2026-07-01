# Wings — website audit business site

Single-file, zero-dependency landing page. `index.html` is the whole site.
Built to practice what it preaches: fast, mobile-first, semantic, with SEO meta
tags and ProfessionalService schema markup baked in.

## Preview it locally
```
cd ~/Desktop/Wings
python3 -m http.server 4399
# open http://localhost:4399 in your browser
```

## Before you go live — replace these placeholders
Search `index.html` for each and swap in your real details:
- `wingsaudits.com.au` → your real domain (appears in canonical, OG, schema)
- `hello@wingsaudits.com.au` → your real contact email
- `ABN [add your ABN]` (footer) → your ABN once registered (free at abr.gov.au)
- Form `action="https://formspree.io/f/your-form-id"` → your real form endpoint
- Pricing ($0 / $149 / from $499) → whatever you decide to charge

## Make the contact form actually send you emails (free)
The form currently posts to a placeholder. Easiest no-code option:
1. Go to https://formspree.io, sign up free, create a form.
2. Copy your form's endpoint (looks like `https://formspree.io/f/abc123`).
3. Paste it into the `action="..."` of the `<form>` in index.html.
Now every enquiry lands in your inbox. (Getform / Web3Forms work the same way.)

## Deploy it (pick one — all free)
- **Netlify Drop**: drag the `Wings` folder onto https://app.netlify.com/drop. Live in seconds.
- **Vercel**: `npx vercel` from this folder, or connect a GitHub repo at vercel.com.
- **Cloudflare Pages / GitHub Pages**: also free, both fine for a static site.

Then point your domain at it and add an SSL cert (all three do this automatically).

## Prove your own scores
Once live, run your own site through https://pagespeed.web.dev — it should score
95–100 on mobile. Screenshot it. "Even our own site scores 100/100" is a great
line in your cold emails.
