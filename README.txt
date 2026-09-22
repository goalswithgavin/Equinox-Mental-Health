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

ADDING PHOTOS
Search index.html for "img-slot" — each one is a placeholder box marked with an
HTML comment like:
  <!-- IMAGE: portrait of Lucia Savage-Reeder — replace this div's content
       with <img src="..." alt="Lucia Savage-Reeder"> -->
There are two: the hero graphic area (currently an SVG, can stay as-is or be
swapped) and the About section portrait. Drop your image files next to
index.html and replace the placeholder div's inner text with an <img> tag,
e.g.:
  <div class="img-slot">
    <img src="lucia-portrait.jpg" alt="Lucia Savage-Reeder">
  </div>

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
Left out on purpose per your note that the business number isn't set up yet.
Once it exists, add it to the "info-list" in the Contact section and to the
footer if you'd like it there too.

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
