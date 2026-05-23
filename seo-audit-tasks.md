# SEO Audit: elteesydney.com.au — Task List
**Audit date:** 25 April 2026 | **Overall SEO Health Score: 47/100**
**Platform:** Shopify | **Industry:** E-commerce + Physical Retail (Period Activewear, Tweens & Teens)

This file is the master task list from the full SEO audit. Use it to ask questions about any recommendation, get implementation details, or mark tasks complete.

---

## 🔴 CRITICAL — Fix immediately

- [ ] **TASK-01** Add H1 tag to the homepage
  - Currently: zero H1 elements on homepage
  - Fix: Add to `index.liquid` in Shopify theme editor

- [ ] **TASK-02** Add JSON-LD schema to the homepage (Organization + LocalBusiness + WebSite)
  - Currently: 0 structured data blocks on homepage
  - Fix: Add to `theme.liquid` inside `<head>` wrapped in `{% if template == 'index' %}`
  - Ready-to-use JSON-LD is available — ask for it

- [ ] **TASK-03** Add LocalBusiness (ClothingStore) schema to Erina store page
  - Currently: No LocalBusiness schema anywhere on the site
  - Fix: Add JSON-LD to `/pages/erina-store` in Shopify
  - Ready-to-use JSON-LD is available — ask for it

- [ ] **TASK-04** Standardise NAP (Name, Address, Phone) across all pages
  - Issues found: address abbreviated on some pages, phone format differs, postcode missing, business name varies
  - Correct standard: `Shop 5, 162 The Entrance Road, Erina NSW 2250` | `(02) 4314 6264` | `Eltee Sydney`
  - Pages to fix: homepage, contact page, Erina store page, store locator

- [ ] **TASK-05** Fix products sitemap returning 0 URLs
  - Currently: `sitemap_products_1.xml` is empty — Google may not be discovering product pages via sitemap
  - Fix: Check Shopify admin > Online Store > Preferences, or use an SEO app to regenerate

---

## 🟠 HIGH — Fix within 1 week

- [ ] **TASK-06** Write meta descriptions for all collection pages and top product pages
  - Currently: Missing on `/collections/girls-period-swimwear`, `/collections/teen-period-underwear`, most PDPs
  - Format: 150-160 characters, lead with keyword, speak to the parent persona
  - Ask for drafts for any specific page

- [ ] **TASK-07** Add FAQPage schema to `/pages/faq`
  - Currently: 30+ Q&A pairs with zero schema — missing featured snippets and PAA appearances
  - Fix: Add FAQPage JSON-LD via Shopify theme or schema app
  - Ready-to-use JSON-LD is available — ask for it
  - Time estimate: 1-2 hours

- [ ] **TASK-08** Extend HSTS max-age from 91 days to 1 year
  - Currently: `max-age=7889238` (~91 days)
  - Fix: Update to `max-age=31536000` in Cloudflare settings

- [ ] **TASK-09** Add AI crawler rules to robots.txt + create llms.txt
  - Currently: GPTBot, ClaudeBot, PerplexityBot not mentioned in robots.txt — no llms.txt file
  - Fix: Add explicit Allow rules for AI crawlers; create `/llms.txt` at domain root
  - Full llms.txt content template available — ask for it

- [ ] **TASK-10** Add phone number, postcode, and email to Erina store page
  - Currently: All three missing from `/pages/erina-store` body content
  - Phone: (02) 4314 6264 | Postcode: 2250 | Email: orders@elteesydney.com.au

- [ ] **TASK-11** Add "Central Coast" keyword to Erina store page (and ideally other pages)
  - Currently: "Central Coast" appears nowhere on the site — invisible for all local Central Coast searches
  - Fix: Add to meta description, add subheading "Serving the Central Coast from Erina", add suburb mentions (Gosford, Terrigal, Avoca Beach, Tuggerah, Woy Woy, Wyong)

- [ ] **TASK-12** Fix OG image URL from http:// to https://
  - Currently: Open Graph image starts with `http://` — triggers mixed content warnings
  - Fix: Update in Shopify theme settings

---

## 🟡 MEDIUM — Fix within 1 month

- [ ] **TASK-13** Add Google Maps embed (iframe) to Erina store page
  - Currently: External Maps link only — no embedded map
  - Fix: Replace or supplement the link with a proper `<iframe>` embed from Google Maps

- [ ] **TASK-14** Add age-to-size guide above the fold on collection pages
  - Currently: Sizing system (e.g. G10-12 = W4) is opaque to parents
  - Fix: One-line guide: "Age 8-10 = G8-10 (W2) | Age 10-12 = G10-12 (W4)..." above product grid

- [ ] **TASK-15** Tighten blog topical focus
  - Currently: Blog mixes period product content with Matildas coverage and Olympic parenting stories
  - Fix: Plan future posts around period care, sport, and tween/teen health — ask for a content plan

- [ ] **TASK-16** Add source citation to the 63.4% / 67% statistic everywhere it appears
  - Currently: Appears on homepage, swimwear collection, teen underwear collection, and a PDP — no source
  - Fix: Add "(Source: Eltee Sydney Survey, 2,302 Australian girls, [year])" with link to research article

- [ ] **TASK-17** Add VideoObject schema to embedded videos
  - Currently: Knicked comparison video and founder video have no schema — missing video rich results
  - Fix: Add VideoObject JSON-LD alongside each embedded video

- [ ] **TASK-18** Fix breadcrumb label on swimwear collection page
  - Currently: Reads "Home / SWIM / Why the Best Teen Period Swim?" (a question as a nav label)
  - Fix: Change to "Home / Swim / Period Swimwear for Girls"

- [ ] **TASK-19** Add ItemList schema to collection pages
  - Currently: No ItemList schema on `/collections/girls-period-swimwear` or `/collections/teen-period-underwear`
  - Fix: Enables product-level rich results (names, prices, ratings) in SERP snippets

- [ ] **TASK-20** Audit and optimise Google Business Profile (GBP)
  - Currently: GBP listing exists (Maps link found) but optimisation status unknown
  - Check: Primary category (should be "Clothing Store"), Saturday hours, address format, phone, website URL pointing to Erina store page
  - Ask for a full GBP optimisation checklist

- [ ] **TASK-21** Add AggregateRating schema to homepage and Erina store page
  - Currently: "220+ Happy Customers, 4.7 stars" shown visually but no schema — no star rich snippets in SERP
  - Fix: Enable schema in your review app (Judge.me, Okendo, etc.) or add manually

---

## 🟢 LOW / STRATEGIC — Plan for 60-90 days

- [ ] **TASK-22** Build a dedicated "First Period Kit" editorial landing page
  - Currently: `/collections/best-first-period-tween-teen-girl` mixes product types without a guided journey
  - Fix: Create a Step 1 / Step 2 / Step 3 experience with Starter 5-Pack as the hero CTA
  - Ask for a content brief and structure

- [ ] **TASK-23** Restructure "Why Girls Quit Sport" article as a citable research page
  - Currently: Survey data buried in a blog post without methodology, source attribution, or Article schema
  - Fix: Add key findings block, Article JSON-LD with author (Sarah Greenaway), citation format
  - Ask for a rewrite plan

- [ ] **TASK-24** Create competitor comparison articles
  - "Modibodi vs Eltee Sydney teens" and "Bonds period underwear for girls vs Eltee Sydney"
  - High-intent, capturable queries — the Knicked article proves this format works
  - Ask for briefs

- [ ] **TASK-25** Add Article / BlogPosting schema with author bylines across all blog posts
  - Currently: Only one post has a Sarah Greenaway byline — no Article schema on any post
  - Fix: Add BlogPosting JSON-LD to `article.liquid` template once — applies to all 36 posts
  - Ask for the code snippet

- [ ] **TASK-26** Run a full citation audit and fix/build Tier 1 directory listings
  - Tools: BrightLocal or Whitespark
  - Directories: Apple Maps, Bing Places, Yellow Pages AU, True Local, White Pages AU, ProductReview.com.au
  - Your on-site NAP inconsistencies have likely propagated into existing citations

- [ ] **TASK-27** Launch a Google Review acquisition campaign
  - Currently: 220+ on-site reviews but Google review count unknown — local pack rankings depend on Google review velocity
  - Fix: Post-purchase email sequence, packaging insert QR code at Erina store, CTA on Erina store page

- [ ] **TASK-28** Create local content targeting priority queries
  - Target pages: "Period underwear stores Central Coast", "Period swimwear for girls in Sydney and NSW", "Swimming with your period — Central Coast swim club resources"
  - Ask for content briefs

- [ ] **TASK-29** Add FAQPage schema inline on collection pages that have FAQ sections
  - `/collections/teen-period-underwear` has an embedded FAQ section — add schema there too

- [ ] **TASK-30** Separate tween vs teen journeys in site architecture
  - Currently: Tween (8-12) and teen (12-16) are conflated — a dedicated tween page would capture a distinct parent search segment
  - Consider: `/collections/tween-period-underwear` or `/pages/period-underwear-tweens`

---

## Context for this session

- Site: https://elteesydney.com.au (Shopify)
- Physical store: Shop 5, 162 The Entrance Road, Erina NSW 2250 | Mon-Fri 9-5, Sat 9:30-12:30
- Phone: (02) 4314 6264
- Products: Period underwear, swimwear, and activewear for tweens and teens
- Serpstat MCP is configured but pending API token fix (token updated to `0fbb242eb44e3ac4651370660d260eb2`, restart required)
- claude-seo skill installed at `~/.claude/skills/seo/`
- GEO score: 41/100 — strong raw content, weak AI-readiness packaging
- Local SEO score: 34/100 — biggest gaps are schema and Central Coast visibility
- SXO score: 52/100 — schema and meta descriptions are the fastest wins
