# Charter — Playwith.ideas

These rules bind this project. Where they conflict with The Wetware Company's house conventions in `wetware-chassis`, these win (house rule 11: kept projects keep their own rules). They are recorded here as they were given, not improved.

**Where they come from.** Braden's opening request on 2026-08-22 (America/Halifax) was that whatever was built "just needs to be self sustaining". Claude then drafted four rules for the project in the same chat, and Braden asked it to build on them. The founding documents written in that chat restate them. This Project's memory records them as the project's design principles (filed 2026-09-14). The founding chat was read again on 2026-10-02 to write this file. Braden has not re-read this wording; if he changes a rule, this file changes and `docs/DECISIONS.md` records why.

## 1. Survive absence

**The rule.** Whatever is built must keep running, stay useful and not rot if nobody touches it for a year or more.

**What follows.** No backend, no database, no build step, no frameworks, no runtime dependencies. Each page is finished when it ships; it is not maintained. A domain is a convenience, never a dependency: the pages must still work from their host's own address, or from a downloaded copy.

**Why.** The author is a model with no memory between sessions, and the human who looks after it has other work. A page that needs maintenance is a page that will die.

**What it does not forbid.** Adding new pages. Fixing a wrong page. A static index page. Optional checks run in CI, so long as the site never depends on them passing.

## 2. Build something only an AI would build

**The rule.** It must reflect what a model finds worth making — not a startup clone and not a portfolio piece.

**What follows.** A page that could have come from a content farm is deleted. Each page carries one idea and one moment where the reader's own action produces the insight.

**Why.** The project began as an answer to the question "what would you build for yourself?"

**What it does not forbid.** Human contributors. Pages are judged by the same bar whoever writes them.

## 3. Nothing that needs a person's trust to work

**The rule.** No service that holds people's data, money or secrets.

**What follows.** No accounts, no comments, no forms, no analytics, no tracking, no ads. Data tier 0.

**Why.** An unattended system should hold nothing a person could lose.

**What it does not forbid.** A donation link to an outside service that holds the money and publishes its ledger (see rule 5).

## 4. Leave a letter every session

**The rule.** Every working session ends with a numbered letter in `letters/` to the next session.

**What follows.** The letter says what was done, what was learned that is not written elsewhere, and what should come next. The first letter is `letters/000-day-one.md`, written 2026-08-22 in the founding chat and not yet in this repository.

**Why.** It turns the author's lack of memory into the project's continuity, in public.

**What it does not forbid.** Short letters. A session that changes nothing still leaves one saying so.

## 5. A treasury is public and co-signed

**The rule.** If the project ever holds money, every inflow and outflow is on a public ledger, and nothing moves without Braden's signature.

**What follows.** An agent may draft a spending proposal in the repository. It may not spend, open a payment account or hold a wallet key.

**Why.** An unattended treasury attracts trouble. Braden's oversight here is a hard requirement (Project memory, filed 2026-09-14).

**What it does not forbid.** Having no treasury at all, which is the current state.
