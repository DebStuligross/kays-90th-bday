# Kay's 90th — Weekend Info Page

**Design spec** · drafted July 29, 2026 · for the Jul 31–Aug 2 gathering

---

## Context

Twenty-five family members are converging on a rented lodge in the Poconos in
two days to celebrate Kay's 90th birthday. The planning so far lives in a
Google Sheet, a Google Slide, a Drive folder, and a long email thread — which
means nobody except Joe and Deb has the whole picture.

This page is the single place guests go for details. Deb sends one email with
the essentials and a link here. The page has to survive being opened on a
phone, in a car, in the Poconos, by someone who is lost.

**Audience:** ages 0 to 90. Wide range of tech comfort. Several guests are
60+; Kay is 90 and uses a walker. Most will read this on a phone. A few will
print it.

---

## Decisions already made

| Question | Decision |
|---|---|
| Privacy | Public URL, but `noindex, nofollow` + non-obvious repo name. **First names only — no last names anywhere.** |
| Cost / contributions | **Omit entirely.** Joe already handled the ask by email. |
| Schedule detail | Loose timeline. Pin only what's actually fixed. |
| Landing experience | Answer box at top, then sections. |

---

## Page structure

### 0 · Header + Answer Box  *(above the fold, no scrolling)*

The four questions someone actually has when they open this:

- **Where?** `121 Whispering Pines, Freeland, PA 18224` — large, tappable,
  opens Google Maps
- **When can I get in?** Check-in **4:00 PM Friday** · Check-out
  **10:00 AM Sunday**
- **Which room am I in?** One tap → jumps to the room list
- **Who do I call?** Joe and Deb, tap-to-call

Plus a warm one-line header: *Kay's 90th · Freeland Lodge · July 31 – August 2, 2026*

### 1 · Sticky nav

`Travel · Bring · Rooms · Meals · Weekend · Contacts`

### 2 · Getting There

- Address + map link, repeated
- Airports: **AVP (Wilkes-Barre/Scranton)** 42 min — closest · **PHL** and
  **EWR** roughly equidistant, ~2 hrs
- Who's driving what, and when
- **Rides board** — offers and open needs, with a clear "call Deb" line.
  The unsolved one: David needs to reach Newark Sunday for a ~5 PM flight.

### 3 · What to Bring  *(highest-utility section on the page)*

The lodge's supply policy is genuinely surprising, so this leads:

**The lodge does NOT provide these — bring your own:**
towels (bath *and* one for the hot tub) · toiletries and shampoo ·
toilet paper · paper towels · trash bags

**Worth bringing:**
charcoal briquettes for the grill · swimsuit · sneakers for the courts ·
sunscreen and bug spray · a folding chair · flashlight

**For the celebration:**
your five questions for Kay · an instrument if you play · a song for karaoke ·
photos or a memory to share

### 4 · Rooms

Eleven bedrooms across three levels. On phone this renders as a **card per
room**, not a wide table — room number, floor, beds, who's in it, and whether
it has a private bath. The floor-plan image from the Google Slide sits at the
top of the section.

Kay is in Bedroom 5, main floor, private bath — noted as the accessible room.

### 5 · Meals

Who's covering what, in order:

| | |
|---|---|
| Fri dinner | *(open — see questions)* |
| Sat breakfast | Mikaelan & Zack — bagels, pastries, cereal |
| Sat lunch | Mikaelan & Zack — grill, with vegetarian options |
| **Sat dinner** | **Catered by Sand Springs. Pickup at 5:45 PM, 15 min from the lodge — needs a driver.** Salad, pasta primavera, Italian baked chicken, roasted pork loin, roasted red potatoes, vegetable medley, broccoli |
| Sat dessert | Clara & Abby — cheesecake and chocolate cake |
| Sun brunch | Mikaelan & Zack |
| Snacks | Deb & Joe |

**Allergies flagged on the page:** shellfish · bananas · finned fish.
Vegetarian options at Saturday's grill.

### 6 · The Weekend

Loose timeline — Friday evening, Saturday morning / afternoon / evening,
Sunday morning. Only the catering pickup is pinned to a clock.

Activity cards for what's planned:

- **Kay's life story** — the Q&A everyone sent questions for. Robert's
  bringing the Tales card set.
- **Singing** — *Dona Nobis Pacem*, music linked from Drive. Ed's bringing a
  guitar; Joe's rigging a karaoke speaker. Bring an instrument.
- **Kubb** — the Viking yard game from Kay's 80th. Joe's bringing it.
- **The grounds** — 8 acres, pickleball and basketball courts, fire pit,
  gazebo, hot tub
- **Indoors** — 12-seat movie theater, pool table, shuffleboard, poker

### 7 · Who's Here

Contact cards, **first names only**, tap-to-call and tap-to-email.

### 8 · Footer

Last-updated date and version, plus a feedback button — same pattern as the
Bloomsburg page.

---

## Look and feel

Deliberately *not* the Bloomsburg navy-and-red. This wants warmth: deep pine
green, warm cream background, a gold accent for the birthday. Summer, woods,
celebration.

**Legibility is a real requirement here,** not a nicety — several guests are
well over 60. Base font 17–18px, generous line height, high contrast, large
tap targets throughout.

Print stylesheet included so the room list and meal plan come out clean on
paper for the fridge at the lodge.

---

## Build

Static `index.html` + `styles.css` — same shape as the Bloomsburg site, so
edits over the next few days are quick and low-risk. Deployed to GitHub Pages
with `noindex` and a `robots.txt`.

Proposed repo: `freeland-weekend-2026` →
`debstuligross.github.io/freeland-weekend-2026/`

The floor plan gets exported from the Google Slide as a PNG and committed
alongside.

---

## Resolved

| Item | Answer |
|---|---|
| Bed linens | **Provided.** Guests bring towels and toiletries only. |
| Friday dinner | Still unplanned — page says so plainly. |
| Catering pickup driver | Unassigned — flagged on the page as the one open job. |
| Dinner-only guests | Charles, Ed & Kim, Eve & Jeff — arriving Saturday in time for dinner. |
| Ben Caroline | One person. Name used verbatim. |
| Eve's husband | **Jeff**, not Ed. Son unconfirmed, so left out. |
| John & Tracey's phone | 484-557-7278. |
| Kay's Sunday ride | Left off the page — being worked out privately. |
| Karaoke speaker | Left off, unconfirmed. |
| Group gift | Skipped. |
| Viking game | Dropped. Croquet, corn hole, and bocce instead. |
| Dress | Casual all weekend; Saturday dinner business casual. Mike shoots the family photo Saturday. |
| Repo | `kays-90th-bday` |

## Still open

- Who drives to Sand Springs for the 5:45 PM Saturday pickup
- Friday dinner
- Whether Eve and Jeff's son is coming
