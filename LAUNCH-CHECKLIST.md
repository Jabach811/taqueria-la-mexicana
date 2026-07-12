# Taqueria La Mexicana — Pitch & Launch Checklist

The site is static HTML (two pages + images), so hosting is **free**. The only
recurring cost is the domain name (~$10–12/year). Here is everything, in order.

---

## Phase 1 — Before you walk in (do this now)

- [ ] **Put a live demo on the internet** so you can show it on a phone at the
      counter, not just a laptop. Easiest free option since the code is already
      on GitHub: **GitHub Pages**.
      1. Go to the repo on GitHub → **Settings → Pages**
      2. Under "Build and deployment", Source: **Deploy from a branch**,
         Branch: **main**, folder **/ (root)** → Save
      3. In ~1 minute the site is live at
         `https://jabach811.github.io/taqueria-la-mexicana/`
- [ ] **Verify the facts on the site against reality** — the 3 addresses, the
      3 phone numbers, and the hours. Owners notice wrong hours immediately and
      it costs you credibility. (Current numbers on the site: (209) 833-8226,
      (209) 833-6343, (209) 207-9219.)
- [ ] **Test on your own phone**: tap every link, make sure the `tel:` links
      open the dialer and the map links open Google Maps.
- [ ] **Decide your price before you go in.** Typical range for a small
      restaurant site like this: a one-time build fee, plus an optional small
      monthly fee if you'll maintain it (menu/price updates). Have both numbers
      ready so you don't negotiate on the spot.
- [ ] Optional but powerful: pull up their current web presence next to your
      demo for the before/after moment.

## Phase 2 — At the pitch

- [ ] Show the live URL on a phone — that's how their customers will see it.
- [ ] Ask two key questions:
      - **Do you already own a domain name?** (If yes: who has the login —
        GoDaddy, Google, wherever it was bought.)
      - **Who should be able to update the menu and prices, and how often do
        they change?**
- [ ] Bring a simple one-page agreement: what's included, the price, who owns
      what, and the ongoing cost. Get a deposit (50% is normal) before launch.

## Phase 3 — They said "me gusta." Now launch it.

### 1. Fix the placeholders (required before going live)

- [ ] The catering form submits to `https://example.com/catering-inquiry`.
      Wire it to something real — easiest options:
      - **Formspree** (free tier): create a form, swap the form's `action` URL
      - Or move hosting to **Netlify** and use built-in Netlify Forms
      - Or simplest of all: make the button a `mailto:` / link to a Google Form
- [ ] The "Read our reviews →" link points to `#reviews-placeholder`. Point it
      at their real Google reviews or Yelp page.
- [ ] Confirm every menu price with the owner — prices drift.

### 2. Buy the domain (~$10–12/year)

- [ ] Pick a name with the owner, e.g. `taquerialamexicanatracy.com` or
      `lamexicanatracy.com`. Check availability at **Porkbun**, **Namecheap**,
      or **Cloudflare Registrar** (all cheap and honest about renewal pricing).
- [ ] **Register it in the owner's name / with the owner's email**, even if you
      manage it. They should own their own name — this builds trust and
      protects them (and you) long-term. Put the renewal date on a calendar.
- [ ] If they already own a domain, get login access instead of buying new.

### 3. Host it for free (pick one)

**Option A — Netlify (recommended):**
- [ ] Sign up free at netlify.com → "Add new site" → "Import from Git" →
      pick the `taqueria-la-mexicana` repo
- [ ] No build command needed (it's plain HTML) — publish directory is the root
- [ ] Every `git push` auto-updates the live site
- [ ] Bonus: Netlify Forms can handle the catering form with zero code

**Option B — GitHub Pages** (fine too, you may already have it from Phase 1):
- [ ] Same setup as Phase 1; custom domain is added under Settings → Pages

**Option C — Cloudflare Pages:** also free, same idea as Netlify.

### 4. Connect the domain

- [ ] In your host's dashboard, add the custom domain
      (e.g. Netlify: Site settings → Domain management → Add domain)
- [ ] It will tell you exactly which DNS records to create (usually a CNAME for
      `www` and an A/ALIAS record for the bare domain). Add those at the
      registrar.
- [ ] Wait for DNS to propagate (minutes to a few hours). HTTPS/SSL is issued
      automatically — no cost, nothing to install.

### 5. Pre-launch walkthrough

- [ ] On a phone: every link, every tap target, both pages
- [ ] `tel:` links dial the right location
- [ ] Map links open the right address
- [ ] Catering form actually delivers a message to the owner's email — send a
      real test
- [ ] Page title / browser tab text looks right when you share the link in a
      text message

### 6. Get them found (this is where the owner sees real value)

- [ ] Update the **Google Business Profile** for all 3 locations with the new
      website URL (if they haven't claimed them, help them claim — it's free
      and huge for a restaurant)
- [ ] Update **Yelp** website link
- [ ] Update **Facebook / Instagram** bio links
- [ ] Have the owner text the link to friends and family — first traffic

### 7. Handoff & maintenance

- [ ] Agree who makes updates (menu prices, hours, holiday closures) and what
      it costs — a small monthly fee, or per-update
- [ ] Make sure the owner has (or you document for them): the domain registrar
      login, the hosting account, and the renewal date
- [ ] Collect the final payment 🎉

---

## Cost summary for the owner

| Item | Cost |
|---|---|
| Hosting (Netlify / GitHub Pages / Cloudflare) | $0 |
| HTTPS certificate | $0 (automatic) |
| Domain name | ~$10–12 / year |
| Your build fee + optional maintenance | your call |
