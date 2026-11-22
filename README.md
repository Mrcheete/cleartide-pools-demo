# One-Page Website Template

## What this is

A reusable business website template in plain HTML, CSS and JavaScript, with no build tools and no framework. Every page pushes the visitor towards one action: calling or WhatsApping the business.

All the text is placeholder. Headings say **Heading**, smaller headings say **Subheading**, the small labels above headings say **Small Label**, and every paragraph describes what to write there. Use those descriptions as the brief when you ask the client for their information.

## Files

| File | Purpose |
|---|---|
| `index.html` | Homepage: hero, about, before-the-job steps, service links, why choose us, contact cards, call-to-action banner |
| `installations.html` | Four service or type sections, each with a photo, a description and a list of requirements or key points (the homepage service links jump here) |
| `quote.html` | Get a Quote page (linked from the homepage's Get a Quote button): WhatsApp and Email buttons at the top, a quote box (phone, area, email, message) that opens WhatsApp with the details filled in, and 5 "what happens next" steps. Change `data-whatsapp="27000000000"` on the form to the client's number |
| `services.html` | Six service cards that open a popup, plus a 4-step process (not linked from the homepage; add a link if the client needs it) |
| `contact.html` | Contact details, map spot and a WhatsApp button (not linked from the homepage; add a link if the client needs it) |
| `style.css` | All styling. Colours, fonts and spacing are variables at the top of the file, so change those first for each client |
| `main.js` | Header that hides while scrolling, footer year, services popup, contact form handler |
| `logo.svg` | Old sample logo, not used. Replace with the client's logo or delete it |

## Matching HTML to CSS

Every section has a number, for example `<!-- ===== HERO [02] ===== -->` in the HTML and `/* ---------- Hero [02] ---------- */` in `style.css`. The same number means the same section. The full list is at the top of `style.css`.

## What to fill in for each client

- **Business Name**, in the header, footer and page titles (`<title>`).
- **Phone and WhatsApp**: replace `27000000000` in every `tel:` and `wa.me/` link with the client's number (country code first, no `+`, spaces or leading 0 in `wa.me`). Replace the visible text "Phone Number".
- **Email**: replace `email@example.com` and the text "Email Address".
- **Address and hours**: "Street, Suburb, City" and "Opening Days, Opening Hours".
- **Social links**: replace each `href="#"` with the client's page, or remove the ones they don't use.
- **Images**: grey boxes saying "Image Here" or "Photo Here or Video Here" mark where photos go. Swap the `<div class="media-placeholder">...</div>` for an `<img>` tag.
- **Logo**: the header shows the business name as text. To add a logo, put an `<img>` inside the `<a class="logo">` link.
- **Meta description**: the `<meta name="description">` line in each page is the text Google shows. Write one sentence per page.

## Before going live

- There is no email form: customers reach the business on WhatsApp. Every WhatsApp link opens with a message already written ("Hi Business Name, I found you on your website and would like a quote."). It's the `?text=` part of each `wa.me` link: put the client's name in place of `Business%20Name` (`%20` is a space, `%2C` is a comma).
- Read every page once to check no placeholder text is left.

## Don't change unless you mean to

- Class names in the HTML (`hero`, `card`, etc.). The CSS and JavaScript depend on them.
- The `<script src="main.js">` tag at the bottom of each page.
