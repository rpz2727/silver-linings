# Silver Linings Massage — launch plan

The website is built and already online at a **private preview address** —
search engines can't find it yet. This is everything left to do before it
becomes the real public site, and who handles each part.

**Preview:** https://rpz2727.github.io/silver-linings/

Two roles:

- **Liz** — supplies the real words and makes a few calls.
- **You** — whoever manages the site files; makes the edits and publishes.

**Where things stand:** design and layout are final. The bio is a placeholder,
and the phone, email, and address on the page are stand-ins. Nothing is public yet.

---

## Phase 1 — Look over the preview  · Liz

Open the preview link on your phone *and* on a computer. Check that everything
reads the way you want it to.

- [ ] Business name, tagline, and logo look right
      *(tagline currently reads "Personalized massage therapy for real relief.")*
- [ ] Service prices are current
      *(Massage $90 / $120 / $160 for 60 / 90 / 120 min · Craniosacral $70 for 45 min)*
- [ ] Hours are current:
  - Monday 11:00am – 7:30pm
  - Tuesday 2:30pm – 7:30pm
  - Wednesday Closed
  - Thursday 9:00am – 1:30pm
  - Friday 9:00am – 1:30pm
  - Saturday 9:00am – 12:30pm
  - Sunday Closed
- [ ] The "Book Now" buttons open the right Square page
      *(silverliningsmassage.square.site)*
- [ ] Write down anything to change — wording, section order, anything missing

## Phase 2 — Hand over the real content  · Liz

This is the main conversation. Nothing goes public until these are in hand.

- [ ] **Your bio** — one to three short paragraphs: your license and training,
      how you work, what a session with you is like. Replaces the
      "Placeholder for bio" box.
- [ ] **The phone number** to publish (the site shows a stand-in right now)
- [ ] **The email address** for the contact section
- [ ] **The exact address**, including suite number, written how you want it shown
- [ ] **How you want to be credited** — currently "Liz Smith, LMT" (a placeholder)
- [ ] **A photo** — optional. Headshot or treatment-room photo. Send the
      original file, not a screenshot.
- [ ] **Reviews** — optional. Send 2–4 short client quotes. Each client must
      give clear permission first (a text or email saying yes is enough).
      Only quotes you have permission for can go on the site.

## Phase 3 — Put the real content in  · You

- [ ] Edit `index.html`: paste in the bio and the real phone, email, address
- [ ] Add the photo and reviews section, if Liz provided them
- [ ] Preview locally, then `git commit` and `git push`
      *(preview link updates ~1 min after each push)*
- [ ] Send Liz the updated preview for a final look

## Phase 4 — Go live  · You, with Liz's sign-off

- [ ] Get Liz's clear "yes, publish it"
- [ ] Remove the `noindex` line from `index.html`
      *(marked with a "DRAFT" comment — removing it lets Google list the site)*
- [ ] `git commit` and `git push`
- [ ] Open the live site once more on a phone and check every link
- [ ] **Check what Google reads off the page** — go to
      <https://search.google.com/test/rich-results>, paste in the live address,
      and run it. It should find one **Local Business** item with no errors.
      That block is what feeds Liz's name, address, phone and hours to Google,
      so it's worth one look. It can only be tested once the site is public —
      the tool has to be able to fetch the page.
      *(If the custom domain in Phase 5 is being used, run this again on the
      final address, since that's the one the page names as its own.)*

## Phase 5 — Custom web address — optional  · You

- [ ] Keep the free address — `rpz2727.github.io/silver-linings`
      *(works today, nothing to buy or maintain)*
- [ ] Or set up a custom domain like `silverliningsmassage.com` — cleaner on
      cards and by word of mouth, ~$12–15/year. Buy the domain, add it in the
      repo's Pages settings, point DNS at GitHub, then turn on "Enforce HTTPS."

## Phase 6 — Send people to it  · Liz + You

- [ ] Add the link to: Square booking profile, Instagram / Facebook, email signature
- [ ] Put it on the business cards at the next reprint
- [ ] **Google Business Profile** — matters most for a local practice. Make sure
      the listing exists, is claimed, and links to the new site.
- [ ] Start asking happy clients for a Google review

---

## Making changes later

Everything on the site is one file: `index.html` in this repo.

1. Edit the file — all the text and prices live right in it.
2. From this folder, run `git commit -am "what changed"` then `git push`.
3. The live site updates in about a minute.
