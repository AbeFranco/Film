# CLAUDE.md — abrahamfranco.com

Standing instructions for this repository. These apply to every session,
without being restated.

---

## Site update pipeline

Update files arrive in `inbox/` as markdown with `type: site-update` in the
frontmatter. When one is present, process it as follows. Do not improvise a
different workflow.

### Order of operations

1. **Read `wiki/marketing-claims-audit.md` first.** It is the source of truth
   for what may be published. An update file does not override it.
2. **Parse the update file** against the schema in `inbox/_template.md`.
3. **Gate every claim** (below). Report what passes and what is held.
4. **Apply the passing changes.** Leave held items untouched.
5. **Show the diff.** Wait for approval.
6. **Push, then verify production.** Fetch the live URL and confirm the change
   is actually there. Staged is not done.
7. **Stamp the update file** — change `status: pending` to
   `status: applied YYYY-MM-DD`, move it to `inbox/applied/`, and record the
   changes in `wiki/marketing-claims-audit.md`.

### The gate

Nothing publishes unless it passes all of these.

- **Status is VERIFIED.** UNVERIFIED items are held and reported, never
  published, never "cleaned up" into something publishable.
- **Evidence resolves.** The path, file, or URL named must actually exist. If
  it doesn't, hold the item and say so.
- **Testimonials have consent GRANTED** with a date and method. NOT ASKED and
  DECLINED are both blocking.
- **Links load.** Check before publishing. A dead link in a proof strip is
  worse than no proof strip.
- **No prohibited claim reappears.** Cross-check every addition against the
  prohibited list in the audit file.

If an item is held, say which one, why, and what would unblock it. Never
substitute your own wording to make a held item publishable.

### Never guess

If the update file leaves something ambiguous — a number, a timeline, a scope,
a deliverable count — stop and ask. Do not fill the gap from another document,
a template, or inference. Getting this wrong has cost real money on this
project.

---

## Standing claims rules

These extend `wiki/marketing-claims-audit.md` and apply to all pages, always.

- No published claim describes an event not personally witnessed.
- No claim implies an event is ongoing, recurring, or institutional when it
  happened once. Check tense and implication, not just literal truth.
- No claim implies customers, licensees, or usage data that do not exist. This
  includes soft forms: "most common," "organizations often," "facilitators
  report," "clients typically."
- Testimonials are attributed accurately, with relationship disclosed where a
  personal connection exists.
- No adjectives about the quality of the work — powerful, moving, compelling,
  impactful. State facts; let them do it.

### Scope of a truth pass

A truth pass covers **every page in the repository**, not the page in front of
you. Orphan pages not in the nav are still publicly reachable and still count.

---

## Publishing

- The site is GitHub Pages, custom domain, served from `main`.
- `CNAME` must contain `abrahamfranco.com`. Verify before and after every push.
- Verify production after every push by fetching the live URL. A commit that
  isn't on the remote hasn't happened.
- Bump the stylesheet version tag when shared CSS changes, so returning
  visitors don't get a cached layout.
