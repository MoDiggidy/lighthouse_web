# lighthouse_web

Static placeholder page for https://lhlabs.co, the public face of Lighthouse Labs.

Purpose: a quiet, credible page for vendors, suppliers, manufacturers and conference contacts who look us up. It does not sell, collect sign-ups, or name any venture, product, category or ingredient. It makes no product, health or efficacy claims; any future copy that does goes through the regulatory review in lighthouse-pk first.

## Approved public copy (2026-10-12)

Reuse this wording exactly on decks, badges, profiles and email signatures so every surface says the same thing.

- Name: Lighthouse Labs
- Descriptor: Consumer brand incubation and company building.
- About: Lighthouse Labs is an incubator that forms and builds consumer companies. We work with specialist partners across development, manufacturing and operations.
- Contact label: Partners and suppliers
- Contact: lighthouse@lhlabs.co

Design: "Beacon" - night navy, a lamp sitting on the stem of the L with a beam that sweeps every 14 s. Footer "Fl W 14s" is nautical-chart notation for a white light flashing every 14 seconds. Chosen by Matt and Jenny on 2026-10-12 from twelve candidates.

## Files

- index.html - the whole page (inline CSS and JS; fonts from Google Fonts)
- favicon.svg, favicon.ico (16/32/48), apple-touch-icon.png (180) - the L-and-lamp mark
- CNAME - custom domain for GitHub Pages; do not edit or delete

## Updating the site

Edit index.html, commit, push to main. GitHub Pages rebuilds in about a minute.

## Hosting, DNS and certificate

- Hosting: GitHub Pages, repo MoDiggidy/lighthouse_web, branch main, path /. Custom domain lhlabs.co. Enforce HTTPS on.
- DNS: managed at GoDaddy.
  - A @ -> 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
  - CNAME www -> modiggidy.github.io
  - MX (Google Workspace mail) and TXT (Google site verification, SPF) records belong to email. Never change them for the website.
- Certificate: Let's Encrypt via GitHub, covers lhlabs.co and www.lhlabs.co, renews automatically.
- If the certificate ever stalls (the Pages API shows no https_certificate, or it stays pending while DNS is correct): clear the custom domain, wait a minute, set it back to lhlabs.co, then enable Enforce HTTPS once the state is approved. This fixed the first issuance on 2026-10-12, which had stalled because the domain was registered with GitHub before DNS pointed there.

## History

Replaced a free GoDaddy Website Builder page on 2026-10-12. Build record: lighthouse-pk council record _system-improvement/council-2026-10-12-lhlabs-placeholder.md and returns LHWEB-01-c through LHWEB-04 in the estate returns folder.
