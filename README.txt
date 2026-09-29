EQUINOX MENTAL HEALTH — WEBSITE
================================

FILES
- index.html — the entire site, fully self-contained. All images (the Equinox
  logo mark, the full logo lockup, the favicon, and your "Built by Gavin
  Reeder" badge) are embedded directly in the file as base64 data, so the
  page will always display correctly no matter how it's moved, unzipped, or
  opened — no separate assets folder required.
- assets/ — the same images as loose PNG files, kept only as originals/backups
  in case you want to reuse them elsewhere. index.html does not depend on
  this folder — you can delete it and the site still works.

PORTRAIT
Lucia's photo is now in place in the About section, embedded the same way as
the logos (base64, so it travels with the file). To swap it for a different
shot later, search index.html for `.img-slot` and replace the `<img>` inside
it with a new one — the box is cropped to a 4:5 ratio, so a similar
portrait-orientation photo will drop in most cleanly.

CONTACT FORM
The "Book an appointment" form currently opens the visitor's email app with a
pre-filled message to lsavagereeder@protonmail.com (a mailto: link) — this
works everywhere but relies on the visitor having a configured email client,
and doesn't guarantee delivery. For something more reliable once this goes
live, worth wiring the form up to a form backend (e.g. Formspree, Basin) or a
real booking tool (e.g. Calendly, SimplePractice's client portal) — happy to
help with that when you're ready.

MOBILE
On small screens the nav collapses into a full-screen menu, and a "Book an
appointment" bar stays pinned to the bottom of the screen so it's always one
tap away — that's the #1 action Lucia wants visitors to take.

CREDIT LINK
There's a small "Built by Gavin Reeder" bar at the very bottom of the page,
with your logo badge next to it, linking to goalswithgavin.vercel.app. Remove
that <div class="credit-bar">...</div> block near the end of index.html any
time you don't want it there (e.g. once you hand the site fully over to the
client).

PHONE NUMBER
(802) 227-4507 is now listed in the Contact section, with a tap-to-call link
for mobile visitors.

COLORS / FONTS USED
- Ink black:      #1A1B17
- Paper white:    #F6F4ED
- Twilight purple:#5B4B78
- Meadow green:   #4B6A4F
- Horizon blue:   #3D6478
- Headline font: Fraunces (Google Fonts)
- Body font: Karla (Google Fonts)
Both load from Google Fonts via the <link> tags at the top of index.html —
keep those if you want the fonts to keep working, or self-host them if you'd
rather not depend on Google Fonts.
