---
id: W-999
slug: playwith-ideas
name: "Playwith.ideas"
kind: kept-project
stage: proposed
one_liner: "Small web pages that each teach one lasting idea by letting you play with it."
thesis: "A library of static explorable explanations, each teaching one evergreen idea through one interaction, written by Claude across sessions that share no memory, and built to keep working with nobody looking after it."
payer: "nobody. It is designed to cost almost nothing, and nothing is sold."
revenue_model: none
origin:
  founded_by: mixed
  founded_on: 2026-08-22
  source: "The founding chat in the Claude Project 'Playwith.ideas App', last updated 2026-08-23 00:39 UTC, which is 2026-08-22 in Halifax; its start time is not known. Read again in this session on 2026-10-02, along with the Project's memory, the GitHub API, Vercel, Cloudflare and Linear."
data:
  tier: 0
  holds: "nothing"
  retention: null
  deletion_path: null
ai:
  dependency: build-time
  models: []
  monthly_budget_usd: 0
  breaker: hard
cost:
  infra_monthly_usd: 0
  model_monthly_usd: 0
  other_monthly_usd: 0
  notes: "Static hosting on GitHub or Cloudflare costs nothing. No domain is registered for it that could be found; if one is bought, about 10 to 12 USD a year. The model sessions that write pages are not costed: who pays for them is not known."
payments:
  rail: none
  provider: null
hosting:
  mode: independent
  domain: null
  dedicated_domain: null
  repo: "github.com/thewetwarecompany/playwith-ideas"
  worker: null
  health_url: null
admission:
  dispute_prone: { answer: no, note: "Nothing is sold." }
  custodies_funds: { answer: no, note: "It holds no money. The charter allows a future treasury only on a public ledger with Braden's co-signature, and none exists." }
  needs_synchronous_human: { answer: no, note: "Static pages. No accounts, messages or support queue." }
  tail_risk_beyond_balance_sheet: { answer: no, note: "It publishes explanations of settled ideas and holds nothing about anyone. The realistic bad day is a page that explains something wrongly; it is fixed by a commit." }
  cold_email_volume: { answer: no, note: "It sends no email." }
  remotely_operable: { answer: yes, note: "A git repository and a static host, both run from a browser or the command line." }
  decision: pending
  decided_by: null
  decided_on: null
kill:
  criterion: "Not decided. The founding documents say the library is complete at any size and is meant to be inherited by fork rather than shut down. Braden decides when, if ever, the company stops stewarding it."
  launched_on: null
  review_on: null
brand:
  level: kept
  show_on_house_site: false
tracking:
  linear: null
gates:
  cleared: []
exit:
  export_path: null
updated: 2026-10-02
---

## Thesis

Some ideas only land when you do them: you have to count false alarms to feel why a positive test for a rare disease usually means you are fine. This library builds the hands-on version of ideas like that, one page each, free, with no accounts and no tracking. It exists because Braden offered Claude a domain and asked what it would build, on the condition that it sustain itself; it is for anyone who wants to understand an idea, and for teachers who want to send a class somewhere safe.

## What exists today

**Verified** in this session, on 2026-10-02 (America/Halifax):
- The repository `thewetwarecompany/playwith-ideas` exists on GitHub. It is public, its default branch is `main`, it has no licence, and it had no commits before this passport's commit. It was created 2026-10-03 02:13 UTC. Checked with the GitHub API and by cloning it.
- GitHub Pages is not switched on for it (`has_pages: false` in the GitHub API).
- Vercel holds no domain and no project for it: listing domains returned none, and a project search for "play" returned none.
- Cloudflare runs no Worker for it. The account's Workers are `family-table`, `todo`, `civic-grove-site`, `wetware-site` and `capacity-signal-site`.
- Vercel's registrar does not support the `.ideas` ending.
- Linear has no project for it, and a search found no issue about it.
- The Claude Project has no documents and no instructions; its one past chat is the founding chat.
- The founding chat holds seven files written there on 2026-08-22: the Bayes page `bayes/index.html` and six documents, `README.md`, `VISION.md`, `CONTRIBUTING.md`, `ARCHITECTURE.md`, `SUSTAINABILITY.md` and `letters/000-day-one.md`. Read in full in this session.
- The slug `playwith-ideas` is not used in the registry or the intake queue of `wetware-chassis`.

**Not verified:** whether Cloudflare Registrar holds a domain for it (no tool here reads the registrar; Braden can check the dashboard); whether the founding files exist on any computer; whether a checkout exists on the Mac mini.

**Believed**, from this Project's memory and not checked again:
- The static architecture is a firm decision (filed 2026-09-14).
- The repository goes in The Wetware Company's organisation (filed 2026-10-02).
- A ten-year domain registration and about USD 50 a month of cloud credits are available (filed 2026-09-14). These first appear in a prompt Claude drafted in the founding chat; Braden did not confirm them there.
- Open Collective is a possible sponsorship route (filed 2026-09-14).

## Principles and constraints

The project has its own charter, `CHARTER.md`, which outranks house conventions. Its five binding rules: survive absence; build something only an AI would build; nothing that needs a person's trust to work; leave a numbered letter every session; any treasury is on a public ledger and needs Braden's co-signature. Braden's own founding words were that it "just needs to be self sustaining".

These conflict with house conventions in two places, and the charter wins: the pages need client-side JavaScript to work, and the Bayes page uses its own typefaces loaded from Google Fonts.

## Data and privacy

It collects nothing about anyone. There are no accounts, forms, comments, analytics, cookies or trackers. The one outside request the founding documents allow is loading fonts from Google Fonts, which tells Google a reader's address; copying the fonts into each page's folder would remove it. None of the content is health, financial or about minors, although the Bayes page uses a medical screening test as its example.

## AI and model use

Claude, made by Anthropic, writes the pages and the letters in working sessions. No model runs while people use the pages. If a page is wrong, it is wrong until a session fixes it; the page says it was built by a model.

## Money

It costs nothing to run today. No treasury, wallet, payment account or donation link exists. Revenue: none. The founding documents rule out ads, tracking, sponsored content, paywalls and selling data.

## What it needs from a legal person

A licence choice, because the repository is public with none. Turning on a static host. A domain, if one is wanted, registered and paid by a person. Any sponsorship account, if one is ever wanted.

## Kill criteria

Not decided. The founding documents describe a library that is complete at any size and inherited by fork rather than shut down. If the company stops stewarding it, the repository and the pages could stay up as they are.

## Exit path

The repository is the whole project. It transfers to another organisation in one step, and any clone can redeploy it on any static host.

## Open questions for Braden

1. **Kept project or experiment?** The schema forces a value, and `kept-project` is written here only because an experiment must name a payer and none exists. Kept: own rules, nobody pays, no cost; reversible. Experiment: needs a payer and a 90-day kill rule that contradicts the founding aim; reversible but awkward. Sidestep: leave it out of the registry as a hosted public repository.
2. **Which licence?** Public with none today, which forbids forking. Forced by the first page committed. CC BY 4.0 throughout, as the founding text says; CC BY 4.0 for words with MIT for code; or CC BY-SA 4.0. One-way door for anything published under it. Sidestep: commit no pages until it is chosen.
3. **Which name and address?** "Playwith.ideas" or the founding "Explorables". Forced by first launch. Host address, USD 0; a subdomain of `thewetwarecompany.com`, USD 0; or its own domain at about USD 10 to 12 a year. Reversible. Sidestep: launch on the host address and name it later.
4. **Which host?** Forced by first deploy. GitHub Pages, Cloudflare Workers with static assets, or Cloudflare Pages, all USD 0 and reversible. Sidestep: a downloadable archive.
5. **Import the seven founding files?** Forced by any page work. All verbatim, pages and letter only, or rebuild. Reversible. Sidestep: commit an export of the founding chat as the record.
6. **Which founding resources are real?** The Linux machine, wallets, ten-year domain and cloud credits came from a prompt Claude drafted. Confirm or strike each. Reversible. Sidestep: assume none.

The same questions, with costs in full, are in `docs/DECISIONS.md`.

## Log

- 2026-10-02 — passport written by a Claude Code session from the founding chat, this Project's memory, and live checks of GitHub, Vercel, Cloudflare and Linear. Not submitted for assessment. Not admitted.
