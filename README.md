# GLP-1 After Denial - Hugo Site

A simple Hugo site for sharing my GLP-1 medication experience and affiliate monetization.

## Quick Start

### Local Development
```bash
# Install Hugo if needed: https://gohugo.io/installation/
hugo server -D
# Site runs at http://localhost:1313
```

### Deploy to Netlify
1. Push to GitHub
2. Connect repo to Netlify
3. Build settings are in netlify.toml
4. Deploy!

Or drag-and-drop the `public` folder to [app.netlify.com/drop](https://app.netlify.com/drop)

## Site Structure

```
content/
├── _index.md              # Homepage
├── articles/
│   ├── my-journey.md      # Personal story
│   ├── glp1-options-ranked.md    # Options comparison
│   └── best-telehealth-glp1.md   # Telehealth platforms
└── resources/
    ├── _index.md          # Resources hub
    └── how-to-reconstitute-peptides.md  # Reconstitution guide
```

## Before Going Live Checklist

- [ ] Replace `AFFILIATE_LINK` placeholders with actual affiliate links
- [ ] Update email in hugo.toml (hello@glp1afterdenial.com)
- [x] Purchase domain (glp1afterdenial.com) ✓
- [ ] Connect domain to Netlify
- [ ] Apply to affiliate programs:
  - [ ] Royal Peptides (quick approval)
  - [ ] Mochi Health or similar telehealth
  - [ ] Consider ShareASale for GLP-1 related offers

## Theme Setup

This site uses [PaperMod](https://github.com/adityatelange/hugo-PaperMod).

To add the theme:
```bash
git init
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

Or download and extract to `themes/PaperMod/`

## Customization

### Update Branding
- Edit `hugo.toml` for site title, description, social links
- Add logo to `static/images/`

### Add New Content
```bash
hugo new articles/new-post.md
```

### Shortcodes Available
- `{{< affiliate-disclosure >}}` - FTC disclosure box
- `{{< cards >}}...{{< /cards >}}` - Card grid wrapper
- `{{< card title="" link="" description="" >}}` - Individual card

## Affiliate Strategy

### Phase 1: Quick Approval
- Apply to Royal Peptides (10% commission, 24-48hr approval)
- Include links in reconstitution guide

### Phase 2: Higher CPA
- Telehealth platforms (Mochi Health, etc.)
- $100-250 CPA per signup

### Phase 3: Expand
- Add more articles targeting long-tail keywords
- Build email list for repeat traffic
- Consider adding a dosing calculator tool

## Content Calendar Suggestions

Week 1-2:
- My Journey (done)
- Options Comparison (done)
- Telehealth Comparison (done)
- Reconstitution Guide (done)

Week 3-4:
- "Insurance Denied My GLP-1 - Now What?"
- "Semaglutide vs Tirzepatide - Which Is Better?"
- "How I Manage Side Effects"

Month 2:
- "Reddit's Favorite Peptide Suppliers Reviewed"
- "LillyDirect Complete Guide"
- "Protein Goals on GLP-1s"

## SEO Keywords to Target

High intent, lower competition:
- "lost ozempic prescription what now"
- "can't afford zepbound alternatives"
- "compounded semaglutide reviews"
- "how to reconstitute semaglutide"
- "telehealth semaglutide no insurance"
- "mochi health vs hers semaglutide"
- "research peptides semaglutide reddit"

## License

Personal use. Not for redistribution.
