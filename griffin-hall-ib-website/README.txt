GRIFFIN HALL · INWARD BOUND — website
=====================================

A six-page static website. No build tools, no accounts. Just open the
files in a browser, or upload them to any web host.

PAGES
-----
  index.html     Home (hero, race explainer, countdown)
  about.html     The sport + Griffin Hall + the coaches
  history.html   Timeline + past-results table
  squad.html     This year's roster, by division
  sponsors.html  Sponsorship tiers + partner wall
  contact.html   Contact details + join form
  styles.css     All styling (colours, fonts, layout)
  app.js         Menu, countdown, form behaviour

TO PREVIEW
----------
  Double-click index.html. It opens in your browser and all the links
  between pages work straight away.

WHAT TO FILL IN
---------------
Anything written in [SQUARE BRACKETS] is a placeholder for you.
Search the files for "[" to find them all. Key ones:

  • Emails & socials — [squad@email.com], @[griffin.ib], the "#" links
    in the footer and on the contact page.
  • Coaches (about.html) — names, roles, short bios.
  • Squad (squad.html) — runners per division; copy a whole
    "div-block" to add more divisions, delete ones you don't field.
  • History (history.html) — the timeline and the results table.
  • Sponsors (sponsors.html) — tier prices/benefits and the logo wall.
  • Countdown date (app.js) — search for "raceDate" and set the real
    drop time. NOTE: months are 0-indexed, so October = 9.

ADDING PHOTOS
-------------
Every dashed box is a photo slot. To fill one, drop an <img> inside it
and delete the placeholder text. Keep class="filled" on the image:

  Before:
    <div class="photo-slot">
      <span class="ps-label">Add a photo</span>
    </div>

  After:
    <div class="photo-slot">
      <img class="filled" src="images/team-2026.jpg" alt="Griffin squad at Endpoint">
    </div>

Put your image files in a folder next to the HTML (e.g. an "images"
folder) and point src at them. Photos crop to fill the frame.

MAKING THE CONTACT FORM WORK
----------------------------
Right now the form just shows a friendly note — it doesn't send email.
Two easy options:
  1. Formspree (formspree.io): create a form, then set the <form> tag's
     action to your Formspree URL and method="POST".
  2. Google Form: delete the form and link a button to it instead.

PUBLISHING IT (free options)
----------------------------
  • GitHub Pages — push this folder to a repo, enable Pages.
  • Netlify or Cloudflare Pages — drag-and-drop the whole folder.
  • Any web host — upload the files; index.html is the home page.

FONTS & COLOURS
---------------
Fonts load from Google Fonts (needs internet). Colours live at the top
of styles.css under ":root" — change --gold, --route etc. in one place
to re-skin the whole site. If Griffin has official colours, swap them in.

A NOTE ON CONTENT
-----------------
The "about the sport" and Griffin Hall sections are written from public
information about Inward Bound and Griffin Hall. Double-check the details
against your own knowledge before publishing — course distances and
event specifics change year to year. This is a squad/fan site, not the
official Inward Bound website (anuinwardbound.com).
