# playwith-ideas — rules for agents working in this repo

A library of static explorable explanations, written by Claude, stewarded by Braden. The charter outranks everything here, and everything here outranks the house conventions in `wetware-chassis`.

Read on demand — do not import these, they cost tokens every session:
`CHARTER.md` (the binding rules; read before changing anything) · `README.md` (what it is and where things are) · `docs/DECISIONS.md` (settled; do not reopen without Braden) · `docs/SPEC.md` (what each part must do, and how to check it) · `intake/PASSPORT.md` (the registry record) · the newest file in `letters/`, once that folder exists.

## Rules

1. **Agents propose; Braden decides.** Never settle anything listed under open questions in `docs/DECISIONS.md` — licence, domain, host, visibility, kept project or experiment, imports, spending. Write a proposal; he decides, and the decision is recorded with where and when he said it.
2. **Status lives in Linear.** This repo holds durable things only: architecture, rules, records, and why decisions went the way they did. Never write open, blocked or next into a file here. No Linear project exists for this yet (checked 2026-10-02); do not create one or file issues unless Braden asks.
3. **Authorisation in Linear is Braden's alone.** Never move an issue to `Approved`. Never add or remove the `approved`, `decided`, `decision` or any route label (`claude-code`, `cowork`, `linear-only`, `braden`). An issue you are asked to file stays in Backlog, unlabelled, and says so in its body.
4. **Static only.** HTML, CSS and JavaScript. No backend, build step, framework, package manager or runtime network call (charter rule 1). A proposal to add any of these goes to Braden with its justification.
5. **One idea per page, one folder per page, one `index.html` per folder.** Folders never depend on each other.
6. **Nothing that holds a person's data, money or secrets.** No accounts, forms, comments, analytics or trackers (charter rule 3).
7. **Leave a numbered letter** in `letters/` at the end of every session that changes the repo (charter rule 4). Never edit an earlier letter; correct it in the next one.
8. **Verify the rendered page, not the code.** Open it at 360 pixels wide and at desktop width, look at it, and work through the checks in `docs/SPEC.md` before saying a page is done.
9. **Never invent a fact.** Not a figure, a date, a user or a decision. Write "Not known." or "Not decided." and name who can settle it.
10. **No secrets anywhere** — not in files, commits, letters or chat.
11. **Commands handed to a person** follow the house paste rules: an explicit `cd` to the Mac mini checkout first, lines joined with `&&`, guards inside the block, no `exit`, no suppressed output, paste-safe characters only.
12. **Before committing, run the house gates** from a `wetware-chassis` checkout: `node scripts/paste-check.mjs`, `node scripts/secret-scan.mjs` and `node scripts/copy-check.mjs` on this repo, and `npm run intake -- check` on `intake/PASSPORT.md`. A change is done when they print CLEAN and READY FOR ASSESSMENT, not on an agent's report.
