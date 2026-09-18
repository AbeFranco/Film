---
type: site-update
date: 2026-09-18
source: Claude Code session — homepage rebuild from Abraham's draft (`~/Downloads/Sept2026_web_update.html`) plus his written corrections, 2026-09-18
status: applied 2026-09-18 (partial). Held items 1–4 are still open, so the file stays in inbox/
supersedes: inbox/2026-09-16-flagship-scope.md
---

# Site update — new homepage (commissioned short documentaries)

**Applied 2026-09-18:** `c0f3ec1`, Pages build verified, production checked. The film plays for a logged-out visitor.

**Still held (open):**
0. ~~The Vimeo embed isn't the film.~~ **Resolved 2026-09-18.** Swapped to `1144664034?h=3d7526e6ea` ("The Blessed Corner Short Documentary Film", 2:37 confirmed from the player, plays logged out). `1151406974` is the anchor testimonial. Both IDs are recorded in the vault audit.
1. Anchor quote. The excerpt hasn't been chosen yet. Abraham marks the cut from the verbatim transcript. The quote section is left out of `index.html`, with only an empty marker comment. Restore markup is in section 7.
2. Bio, second sentence. The station call letters are missing, so the whole sentence is left out of the page (empty marker only). The full text is below in section 1. Rewording it to drop the call letters isn't allowed.
3. TAPB category ("best edited video, Division 4"). Held on Abraham's instruction until he checks the certificate. It isn't on the page in any form.
4. Four public-comment testimonials (Emily M., Natalie A., Angela H., Stacy M.), consent NOT ASKED. They're removed from `blessed-corner.html` and `use.html`, not commented out, because comments are public in the page source. That takes them off live. Their text is in git history.

Everything else passed the gate and is applied in the working tree. See the gate report in the session transcript and in the vault audit (addendum 2026-09-18, homepage rebuild).

---

## Supersessions — settled, do not re-ask

Abraham's 2026-09-18 corrections win over every earlier answer and document.

| Earlier position | Now |
|---|---|
| Delete the year structure (2026-09-16 hold, section 5) | **Twelve-month engagement.** The deletion was about the seventeen-film count, not the timeline. The structure is Month 2 premiere, Month 8 call, Month 9 Day of Honor plus the second premiere, photographs throughout, the book at close. |
| Premiere in month one (Sep 8 doc) vs. month two (09-08 answer) | **Month 2.** |
| `[FLAGSHIP_DELIVERY]` | **Obsolete.** The Month 2 and Month 9 structure replaces it. Framed as premieres, not deliveries. |
| Test Run delivery "fifteen days" | **Three weeks from the shoot.** |
| Locked CTA `Start the Test Run — $4,500` with `Applies in full toward the $25,000 campaign` beneath | **Button text is exactly `Start the Test Run`.** No price and nothing beneath it. The rollover sentence sits in the tier body. |
| Portal and curriculum in the $25,000 scope (rate sheet) | **Off the page.** |
| Sep 8 pricing-fix doc vs. Sep 6 rate sheet | **The Sep 6 rate sheet wins.** 1-day shoot, from $100,000, Mr. Curtis stays. |
| Travel "$0.55/mi beyond the Permian Basin" (Abraham's first draft) | **"Travel billed at $0.55 per mile"**, with no radius qualifier. |
| "One film they're still sharing in five years" | **"Same money. Something still working after the event is over."** |
| Nav without Home (first draft) | **Home is restored on every page.** |
| Bio "Seven years in the marketing department… work for a CBS affiliate" | **"Seven years at UT Permian Basin, most recently as digital officer. Before that, a videographer at [call letters], a CBS affiliate, where I won Texas Associated Press Broadcasters awards three years running, 2010 through 2012."** Self-stated. |
| Quote: full ninety words | **An excerpt, cut by Abraham.** 26px, centered, max-width 540px. |

**Banned on the site:** the phrase "unsung hero". It's the bonus film's reveal.

**Bonus film:** the site teases it and doesn't name it. The contract clause lives in the vault at `freelance-clients/Process/commissioned-work-contract-clauses.md`, not on the page.

---

## 1. Claims to add

### Claim
- **text:** "One day on location. One short film about one person. Five finished photographs. Delivered three weeks after the shoot. Applies in full toward the $25,000 campaign."
- **page:** index.html · **placement:** Test Run tier
- **status:** VERIFIED
- **evidence:** `community-impact-campaign-rate-sheet.pdf` (2026-09-06), page 1: 1-day shoot, micro-documentary, 5 photos, 100% rollover. The three-week delivery is Abraham's answer from 2026-09-18. Copy in the vault at `digital-product/Inputs/evidence/`.

### Claim
- **text:** "Travel billed at $0.55 per mile."
- **page:** index.html · **placement:** Test Run fine print
- **status:** VERIFIED · **evidence:** rate sheet page 1, "+ $0.55/mi travel"

### Claim
- **text:** $25,000 tier: "The documentary. The day the community shows up, filmed as it happens, cut into a second short you can send the same week. And a printed book of what that person built, for them to keep." Fine print: "Twelve months. $20,500 after a test run."
- **page:** index.html · **placement:** flagship tier
- **status:** VERIFIED
- **evidence:** rate sheet page 2 (documentary, Day of Honor plus reaction montage, Legacy Book, $20,500 rollover balance). The twelve months is Abraham's answer from 2026-09-18.

### Claim
- **text:** Regional: "Multi-city, broadcast length, full distribution." "From $100,000"
- **page:** index.html · **status:** VERIFIED · **evidence:** rate sheet page 2

### Claim
- **text:** The year section: Month 2, Month 8, Month 9, Throughout, At close (exact copy in `index.html`)
- **status:** VERIFIED · **evidence:** Abraham's answer, 2026-09-18 (the supersessions table above)

### Claim
- **text:** "Midland ISD posted it — 1,300+ reactions, 184 shares. Fannin Elementary posted it separately and drew 181 more. Chick-fil-A Midland shared it too. Nobody coordinated any of that. The Odessa American ran a feature."
- **page:** index.html · **placement:** proof strip
- **status:** VERIFIED
- **evidence:** `Midland ISD shares high engagement numbers.PNG`, `Fannin Elem main FB post engagement numbers.PNG`, `Chic Fil A Midland shared his video.PNG`. For "independently", see the audit's new verified facts from 2026-09-04. The Odessa American URL is below.

### Claim
- **text:** "Seven years at UT Permian Basin, most recently as digital officer."
- **page:** index.html · **placement:** bio
- **status:** VERIFIED (self-stated by Abraham, 2026-09-18; "digital officer" is corroborated by the Odessa American headline)

### Claim — HELD
- **text:** "Before that, a videographer at [STATION CALL LETTERS], a CBS affiliate, where I won Texas Associated Press Broadcasters awards three years running, 2010 through 2012."
- **status:** self-stated. **Held** because the call letters are missing. This unblocks when Abraham supplies them.

## 3. Testimonials

### Testimonial — HELD (excerpt pending)
- **quote:** an excerpt of the AnchorTestimonial.mov transcript. The exact cut is to be marked by Abraham.
- **name:** Mary Kate Hamilton · **role:** anchor and reporter, CBS7 / First Alert 7 News
- **said_on:** on camera, May 12, 2025, at Mr. Curtis Day
- **source:** `digital-product/Inputs/evidence/mr-curtis-testimonials.txt` (vault)
- **consent:** GRANTED · **consent_date:** before recording, on camera, for marketing use (recorded in the audit 2026-09-09)
- **page:** index.html

### Testimonials — HELD, consent NOT ASKED
- Emily M., Natalie A. (`blessed-corner.html`), and Angela H., Emily M., Stacy M., Natalie A. (`use.html`). All removed. Restore each one from git history once consent is GRANTED, with a date and a method.

## 4. Links

### Link
- **url:** https://www.oaoa.com/local-news/utpb-digital-officer-creates-short-documentary/
- **anchor_text:** Odessa American · **page:** index.html · **placement:** proof strip
- **verified_live:** 2026-09-04 in a browser (curl gets a 403 from a bot block). Re-checked 2026-09-18, see the audit.

## 5. Copy changes

- `index.html`: replaced in full with the new page.
- Nav: Home / The Blessed Corner / Contact on every page. The other pages already had this. The new `index.html` gets it too.

## 7. Open questions

- To restore the quote: the section markup is `<section><div class="wrap"><blockquote>&ldquo;EXCERPT&rdquo;</blockquote><p class="attrib">Mary Kate Hamilton, CBS7 &middot; on camera, May 2025</p></div></section>`, placed after "How the story gets found". The CSS is already in the page.

## 8. Do not touch

- `licensing.html`, `sponsorship.html`, and the remaining flagged `use.html` copy. Those are separate decisions still pending.
