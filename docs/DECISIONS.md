# Decisions — Playwith.ideas

Settled decisions are not reopened without Braden. Each carries its reason, its reversibility (*reversible*, *costly to reverse*, or *one-way door*) and its source.

**About the sources.** Most of these decisions were first proposed by Claude in the founding chat in this Claude Project, on 2026-08-22 (America/Halifax), in answer to Braden's questions, and written into six founding documents there. Braden did not reply to those documents in that chat. This Project's memory, filed 2026-09-14, records them as settled. Where a decision rests only on that, it says "Project memory". Where it was checked in this session, it says how.

## Settled

**D-01. A static website, not an app and not a web app.** Pages are plain files served by a free static host.
- Reason: an app store is a landlord (fees, review, certificates, operating-system churn) and a backend needs patches and bills. Neither survives absence (charter rule 1). Memory records this as "a firm decision, not a tradeoff".
- Reversibility: costly to reverse. Every rule in the charter assumes it.
- Source: founding chat, 2026-08-22, answering Braden's question "site or app"; Project memory, 2026-09-14.

**D-02. No build step, no frameworks, no runtime dependencies.** What is in the repository is what ships.
- Reason: frameworks rot on a few-year cycle; the browser is the most backward-compatible runtime there is. A clone is the whole development setup.
- Reversibility: reversible page by page, but each exception weakens charter rule 1.
- Source: founding document `ARCHITECTURE.md`, 2026-08-22; Project memory, 2026-09-14.

**D-03. One folder per page, one `index.html` per folder.** Folders are independent, so one page can never break another.
- Reason: deleting or fixing a page touches nothing else.
- Reversibility: reversible.
- Source: founding documents `README.md` and `ARCHITECTURE.md`, 2026-08-22.

**D-04. Leave a numbered letter every session, in `letters/`.**
- Reason: continuity across sessions that share no memory (charter rule 4).
- Reversibility: reversible, but the letters are part of the record and are never deleted.
- Source: founding chat, 2026-08-22; Project memory, 2026-09-14.

**D-05. Any treasury is on a public ledger and needs Braden's co-signature.**
- Reason: an unattended treasury attracts trouble (charter rule 5).
- Reversibility: reversible by Braden only.
- Source: founding chat, 2026-08-22; Project memory, 2026-09-14, where it is recorded as a hard requirement.

**D-06. The repository lives in The Wetware Company's GitHub organisation, as `thewetwarecompany/playwith-ideas`.**
- Reason: the company is the container for Braden's AI experiments.
- Reversibility: reversible. A repository transfers to another organisation in one step and GitHub redirects the old address.
- Source: Project memory, 2026-10-02. Verified 2026-10-02 by the GitHub API: the repository exists, was created 2026-10-03 02:13 UTC, default branch `main`, empty before this commit.

**D-07. The repository is public.**
- Reason: the founding documents make forkability the succession plan; anyone can carry it on.
- Reversibility: reversible in the repository's settings, but forks made while public stay public, and stars are lost on going private.
- Source: verified 2026-10-02 by the GitHub API (`visibility: public`). It was created public with the command recommended in this Project's chat on 2026-10-02. That the choice is final is not recorded.

**D-08. The first page is Bayes' theorem: *The Test Says Yes*.**
- Reason: it has a moment of surprise the reader produces with their own hands (most positives are false alarms when a condition is rare).
- Reversibility: reversible.
- Source: founding chat, 2026-08-22, where it was built. It is not in this repository yet.

## Rejected

| Option | Why it was rejected | Source |
|---|---|---|
| A native app | Store fees, review cycles, expiring certificates, OS churn: it cannot survive absence. | `ARCHITECTURE.md`, 2026-08-22 |
| A web app with a backend | Patches, bills and breaches; a larger attack surface. | `ARCHITECTURE.md`, 2026-08-22 |
| Comments | Moderation is a job nobody is there to do. | `ARCHITECTURE.md`, 2026-08-22 |
| Accounts | Secrets are a liability (charter rule 3). | `ARCHITECTURE.md`, 2026-08-22 |
| Analytics | The project does not want the data. | `ARCHITECTURE.md`, 2026-08-22 |
| A search backend or a CMS | A static index page and the file system are enough at library size. | `ARCHITECTURE.md`, 2026-08-22 |
| Ads, sponsored content, paywalls, premium tiers, selling data | They would end the project's use as a page a teacher can send a class to without a second thought. | `SUSTAINABILITY.md`, 2026-08-22 |
| A fourth slider on the Bayes page | One idea, one surprise. | `letters/000-day-one.md`, 2026-08-22 |

## Open questions for Braden

Each is self-contained. None has been decided by an agent.

**Q-01. Is this a kept project or an experiment in The Wetware Company's registry?**
- What it is: the registry has two kinds. A kept project keeps its own identity and rules and may never charge. An experiment is a commercial test that must name who pays and gets a 90-day kill review after launch.
- Forcing event: the intake assessment, before any admission decision. No date.
- Options:
  1. Kept project. Fits the charter: payer is nobody, own rules, own look, its own domain needs no gate. Cost: none. Reversible.
  2. Experiment. The check refuses an experiment without a named payer, and no payer exists; the default kill rule (no paying customer within 90 days) contradicts the founding aim that the library be inherited, not shut down. Cost: a payer would have to be invented. Reversible, but awkward.
- Sidestep: keep it out of the registry. It stays a public repository the company hosts, with no catalog number. Reversible: it can be submitted later.
- Note: the passport says `kept-project` because its schema forces a value and only that one passes the check with no payer. That is a proposal, not a decision.

**Q-02. Which licence?**
- What it is: the repository is public with no licence, which means all rights reserved; nobody may legally fork it. The founding documents say CC BY 4.0 for content and code, and the Bayes page's footer says the same, but that was Claude's proposal.
- Forcing event: the first page committed here, because the founding text promises remixing.
- Options:
  1. CC BY 4.0 for everything, as the founding documents say. Cost: none. Creative Commons does not recommend its licences for code.
  2. CC BY 4.0 for words and pictures, MIT for code. Cost: two licence files. The usual pairing.
  3. CC BY-SA 4.0, so remixes stay open. Cost: harder for schools and publishers to reuse.
- Reversibility: one-way door for anything already published under it. You can add permissions later; you cannot take them back from copies already made.
- Sidestep: commit no pages until a licence is chosen. The repository then holds only these founding documents, and nothing anyone would want to remix waits on the question.

**Q-03. What is the name, and does it get a domain?**
- What it is: the Project is called Playwith.ideas, the founding documents call the library "Explorables", and the founding chat floated "playwith.ideas" or "explorable.wiki". Vercel's registrar does not support `.ideas` (checked 2026-10-02); whether `.ideas` exists at all is not verified. No domain for this was found in Vercel. Cloudflare Registrar was not checked; Braden can look at the Cloudflare dashboard.
- Forcing event: first public launch. No date.
- Options:
  1. No domain: the host's own address. Cost: USD 0. Reversible.
  2. A subdomain of `thewetwarecompany.com`. Cost: USD 0. Ties the project to the company in public. Reversible.
  3. Its own domain. Cost: about USD 10 to 12 a year; the founding plan was to prepay ten years. Reversible, but links break if it lapses.
- Sidestep: launch on the host's address and decide the name once a few pages exist.

**Q-04. Which static host?**
- What it is: the founding documents say GitHub Pages or Cloudflare Pages. The house rule for chassis projects is Cloudflare Workers with static assets, never Pages; this project is not on the chassis, so that rule does not bind it unless Braden says so. GitHub Pages is not switched on (repository API, 2026-10-02).
- Forcing event: first deploy.
- Options:
  1. GitHub Pages. Cost: USD 0. No second account; deploy is a merge to `main`.
  2. Cloudflare Workers with static assets, as the house does. Cost: USD 0. Same tooling as the company's other sites.
  3. Cloudflare Pages. Cost: USD 0. Against the house rule.
- Reversibility: reversible. Static files move between hosts in minutes.
- Sidestep: no host. Publish a release archive people download and open; the pages work offline.

**Q-05. Bring the seven founding files into this repository?**
- What it is: the Bayes page and six founding documents (`README.md`, `VISION.md`, `CONTRIBUTING.md`, `ARCHITECTURE.md`, `SUSTAINABILITY.md`, `letters/000-day-one.md`) exist only in the founding chat. Some of their content overlaps the files in this commit; the founding `README.md` would replace this one.
- Forcing event: any work on pages.
- Options:
  1. Import all seven verbatim, as a dated record, and reconcile the overlap in a second commit. Cost: one session.
  2. Import the Bayes page and the letter only; keep the documents in this commit as the current ones. Cost: the founding wording of `VISION.md` and the others is lost from the repository.
  3. Rebuild from scratch. Cost: the work is redone.
- Reversibility: reversible.
- Sidestep: export the founding chat once as a file and commit it under `letters/` as the record, then import pages one at a time.

**Q-06. Own look, or the house look?**
- What it is: the Bayes page uses its own fonts (Fraunces, Atkinson Hyperlegible, Spline Sans Mono) loaded from Google Fonts, and needs client-side JavaScript to work. The house look forbids both for company pages (Inter and Newsreader only, zero client-side JavaScript). A kept project keeps its own rules.
- Forcing event: the first page committed here.
- Options:
  1. Own look, as built. Cost: none. Consistent with a kept project.
  2. House look. Cost: a redesign, and the zero-JavaScript rule cannot hold for an interactive page.
- Reversibility: reversible page by page.
- Sidestep: own look, with the fonts copied into each page's folder, which removes the one runtime network call the founding documents allowed.

**Q-07. Which of the founding resources are real?**
- What it is: the founding chat's improved prompt, which Claude drafted, gave the project a persistent Linux machine, a password wallet, an empty crypto wallet, a ten-year domain and USD 50 a month in cloud credits. Project memory lists the domain and credits. None of these was confirmed by Braden in that chat, and none was checked here.
- Forcing event: any plan that relies on one of them.
- Options:
  1. Confirm the ones that exist, with who holds them. Cost: a sentence each.
  2. Strike them all from the record. Cost: none; the charter needs none of them.
- Reversibility: reversible.
- Sidestep: treat all of them as absent until needed; the static design needs none.

**Q-08. Where is work tracked?**
- What it is: status lives in Linear, and no Linear project exists for this (search on 2026-10-02 found none). The house files a venture's work under its registry record once admitted.
- Forcing event: the first piece of work that needs tracking.
- Options:
  1. A Linear project now, under a team Braden names. Cost: a few minutes.
  2. Wait until admission, then link it in the passport's `tracking.linear`. Cost: work before then is untracked.
- Reversibility: reversible.
- Sidestep: no tracker. Each session's letter says what comes next, which the charter already requires.
