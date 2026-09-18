# inbox — how site updates get onto abrahamfranco.com

Nothing goes on the website by hand. Changes go through this folder.

## To make a change

1. Copy `_template.md` to a new file in this folder. Name it
   `YYYY-MM-DD-short-topic.md`.
2. Fill in only the sections you need and delete the rest. Every claim needs a
   status (VERIFIED or UNVERIFIED) and a source. Every testimonial needs
   consent marked GRANTED, with the date and how they agreed.
3. Leave `status: pending` at the top.
4. Open Claude Code in this repo and say: "process the inbox."

## What happens next

Claude follows `CLAUDE.md` in the repo root:

- Checks every item against the marketing claims audit in the vault
  (`wiki/marketing-claims-audit.md`).
- Publishes what passes. Holds what doesn't, and tells you why and what would
  unblock it. It won't reword a held item to sneak it through.
- Stops and asks if anything is vague: a number, a timeline, a scope.
- Shows you the diff, pushes after you approve, then checks the live site.
- Marks the file `status: applied YYYY-MM-DD` and moves it to `applied/`.

A file that is only partly applied stays in this folder with the held items
listed at the top, so it's obvious what's still open.

## Private by design

This folder and `CLAUDE.md` are excluded from the published site in
`_config.yml`. They live in the repo, not on abrahamfranco.com. Don't remove
that exclusion.
