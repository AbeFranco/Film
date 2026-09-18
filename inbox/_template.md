---
type: site-update
date: 2026-09-16
source: Claude conversation — [topic]
status: pending
---

# Site update

Fill in only the sections you need. Delete the rest. Anything left as a
placeholder will be treated as incomplete and held, not guessed at.

Every factual claim needs a status and a source. No exceptions — this is the
gate that stops retracted claims from reaching production again.

---

## 1. Claims to add

Each entry needs all five fields. An entry missing `status` or `evidence` is
held and reported, never published.

### Claim
- **text:** the exact sentence as it should appear on the page
- **page:** index.html
- **placement:** proof strip, under the film
- **status:** VERIFIED | UNVERIFIED
- **evidence:** path in the evidence folder, or a live URL, or the name of the
  file/transcript that proves it

---

## 2. Claims to remove

### Claim
- **text:** the exact sentence currently on the page
- **page:** which file
- **reason:** why it's coming out — retracted, unverifiable, implies a customer
  that doesn't exist, tense implies something ongoing that isn't

---

## 3. Testimonials

Consent is a separate question from whether they said it. Both are required.

### Testimonial
- **quote:** exact words, transcribed, not paraphrased
- **name:** full name as it should appear
- **role:** title and organization
- **said_on:** date and context
- **source:** transcript file or recording path
- **consent:** GRANTED | NOT ASKED | DECLINED
- **consent_date:** when they agreed, and how (text, email, on camera)
- **page:** where it goes

---

## 4. Links

### Link
- **url:** full URL
- **anchor_text:** what the link should say
- **page:** which file
- **placement:** where on the page
- **verified_live:** date you last confirmed it loads

---

## 5. Copy changes

### Change
- **page:** which file
- **section:** heading or identifiable location
- **old:** current text, exact
- **new:** replacement text, exact
- **reason:** why

---

## 6. New pages

### Page
- **filename:** proposed name
- **purpose:** one line
- **nav:** does it go in the nav, yes or no
- **content:** the copy, or a note that it's coming separately

---

## 7. Open questions

Things Claude Code must ask about rather than decide. Anything here blocks the
push until answered.

- Question, and what's riding on it

---

## 8. Do not touch

Pages or sections that are out of scope for this update, so nothing gets
"improved" along the way.

- filename — reason
