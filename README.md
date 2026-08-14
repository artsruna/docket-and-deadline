# Docket & Deadline — launch guide

Everything in this folder is done. Here's what's left, and it's all things
only you can do (they require your own identity/accounts) — figure on
1-2 hours total, then it mostly runs itself.

## 1. Pick a real domain (~10 min, ~$12/yr)
`docketanddeadline.com` is a placeholder used in the code (canonical tags,
sitemap.xml, robots.txt). Check availability on Namecheap or Porkbun and
buy whatever's free — then find/replace that domain in every `.html` file,
`sitemap.xml`, and `robots.txt`.

## 2. Host it for free (~15 min)
This is a static site — no server needed. Easiest options:
- **Netlify** (netlify.com) — drag the whole `site` folder onto their
  dashboard, done.
- **GitHub Pages** — push this folder to a GitHub repo, enable Pages in
  repo settings.
Either one connects to your custom domain for free once you point your
domain's DNS at them (they'll show you the exact records to add).

## 3. Submit to Google (~10 min, so people can find it)
- Create a free Google Search Console account, verify your domain, and
  submit `sitemap.xml`. This is what gets pages indexed — without it,
  Google may take months to find the site on its own.

## 4. Turn on ads (~15 min to apply, approval takes days-weeks)
- Apply for **Google AdSense** (adsense.google.com) with your new domain.
  New sites are sometimes rejected for "not enough content" — if that
  happens, wait until you've added a few more form guides, then reapply.
- Once approved, AdSense gives you a snippet of code. Paste it into the
  `.ad-slot` divs in each HTML file (search for `class="ad-slot"`), replacing
  the placeholder text.
- Realistic expectations: ad revenue is roughly proportional to visitors.
  A handful of pages with no promotion might see very little for months.
  Growth mainly comes from adding more forms (more search terms you rank
  for) and, ideally, a few backlinks — e.g. mentioning it once on a law
  school forum, subreddit (check self-promo rules), or LinkedIn post.

## 5. Growing it later (optional, whenever you have a spare hour)
The site is built so adding a form is copy-paste-edit, not a rebuild:
1. Duplicate any file in `forms/` as a template.
2. Swap in the new form's content following the same section structure
   (What it does / Before you file / Step-by-step / Common mistakes /
   Filing snapshot sidebar).
3. Add one `<a class="docket-row">` entry to `index.html` in the right
   category, and one `<url>` line to `sitemap.xml`.
High-value forms to add next, given real search volume: FL-100 (divorce
petition), DV-100 (restraining order), CIV-050 (substitution of attorney),
POS-010 (proof of service).

## Honest bottom line
This can become a small, low-maintenance income source, but "generates
money by itself" only kicks in *after* it has traffic — and traffic is
earned, not automatic. The realistic path is: launch it, submit the
sitemap, add 2-3 more forms every so often, and let a year of accumulated
search traffic do the compounding. It will not replace an income in the
first month.
