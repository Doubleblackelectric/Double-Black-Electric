Double Black Electric Inc. — Static Website
=============================================

WHAT'S INCLUDED
---------------
  index.html        Home page
  services.html     Our Services page
  contact.html      Contact page
  css/styles.css    All styling — colors, layout, responsive breakpoints
  js/main.js        Mobile nav toggle + footer year
  assets/           Logo + image folder (drop your logo PNG here)


============================================
LOGO  (already installed)
============================================

Your real logo is already in place — converted from the White.pdf you
sent into clean SVG (vector, scales perfectly) plus PNG fallbacks.

Files in assets/:
  logo-white.svg    — white version, used on dark backgrounds (main site)
  logo-white.png    — 1024px PNG fallback of the white version
  logo-black.svg    — black version, use on light backgrounds if needed
  logo-black.png    — 1024px PNG fallback of the black version
  logo-source.pdf   — your original vector file, kept for reference

To adjust how big the logo appears:
  Open css/styles.css and change these values:
     .brand__logo  { height: 58px; ... }     (nav bar)
     .hero__logo   { width: 220px; ... }     (hero centerpiece)
     .about__logo  { width: 170px; ... }     (about section)


============================================
STEP 2 — (OPTIONAL) SWAP THE HERO MOUNTAIN PHOTO
============================================

The hero background is pulled from Unsplash (a free stock photo site,
no attribution required, commercial use OK).

To use your own photo — a real Mt. Currie shot, for example:

  1. Save the photo into the assets/ folder as:
         assets/hero.jpg            (aim for at least 2000px wide)

  2. Open css/styles.css and find the line near the top:
         --hero-photo: url('https://images.unsplash.com/...');

  3. Replace that line with:
         --hero-photo: url('../assets/hero.jpg');

That will change the background in the hero, services section, and about
section all at once.


============================================
HOSTING THE SITE
============================================

This is a plain static site — drag the folder onto any of these (most free):

  • Netlify           netlify.com  (drag the folder onto app.netlify.com/drop)
  • Cloudflare Pages  pages.cloudflare.com
  • GitHub Pages      pages.github.com
  • Vercel            vercel.com
  • Traditional web host via FTP (Bluehost, SiteGround, etc.)

Netlify's drag-and-drop is the fastest — live in under a minute. Then
point doubleblackelectric.ca at it via a DNS change with your registrar.


============================================
ADDING A CONTACT FORM LATER
============================================

  • Netlify Forms      free, works if you host on Netlify
  • Formspree          free tier, works on any host
  • Web3Forms          free tier, works on any host


============================================
CUSTOMIZING COLORS / FONTS
============================================

Open css/styles.css. At the very top of the file there's a :root block
with CSS variables:

  --bg, --ink, --accent (the yellow), --hero-photo, etc.

Change --accent to swap the highlight color site-wide.

Fonts come from Google Fonts (Oswald for headings, Inter for body).
To change them, edit the <link> tag in each HTML file's <head> and
update the font-family rules in CSS.


============================================
CONTACT INFO ON THE SITE
============================================

Phone, email, and name appear in three places per page
(hero / contact card / footer). To update, search-and-replace across
the three HTML files:

  • 1-778-200-1123
  • James@doubleblackelectric.ca
  • James Pearse
