# Playwith.ideas

A library of small, static web pages that each teach one lasting idea by letting you play with it. You drag a slider, count what happens, and find the idea before anyone names it. The pages are pure HTML, CSS and JavaScript, with no backend, no accounts and no tracking, so they can keep working for years after anyone last touched them. The library was designed and is written by Claude, a model made by Anthropic, working in sessions that share no memory and leave each other letters. A human steward, Braden Root-McCaig, does what needs a legal person. The repository sits under The Wetware Company's GitHub organisation.

## Who it is for

Anyone who wants to understand an idea such as probability, feedback or compound growth, on any device, without signing up for anything. Teachers who want a page they can send a class to and remix.

## Current state

There is no code in this repository yet. This first commit holds the founding documents only.

One working prototype exists: *The Test Says Yes*, a page on Bayes' theorem in which 1,000 dots stand for people and three sliders set how rare a condition is and how good the test is. It was written on 2026-08-22, together with six founding documents, in a Claude chat in the Playwith.ideas Project. Those seven files live in that chat and nowhere this repository can see. Whether a copy exists on any computer is not known; Braden can say. Bringing them in is an open question in `docs/DECISIONS.md`.

Nothing is deployed. No domain is registered for it that could be found.

## Layout

| Path | What it holds |
|---|---|
| `README.md` | This page. |
| `CHARTER.md` | The project's binding rules. They outrank the house conventions. |
| `CLAUDE.md` | Rules for agents working here. |
| `docs/DECISIONS.md` | Settled decisions, rejected options, and open questions for Braden. |
| `docs/SPEC.md` | What the library does, part by part, with a check for each part. |
| `intake/PASSPORT.md` | The record this project carries to The Wetware Company's registry. |

Planned, from the founding documents and not yet here: one folder per page holding one `index.html`, such as `bayes/`, and a `letters/` folder holding one numbered letter per session.

## How to run it

There is nothing to run yet. Once a page is in the repository, each page is one file that opens in a browser with no build step.

To serve the pages on the Mac mini, run this in Terminal. It assumes a checkout at `/Users/braden/Projects/playwith-ideas`, which is not verified, and it stops if the Bayes page is not there. The success line is `Serving HTTP on`, after which the page is at `http://localhost:8000/bayes/`.

```
cd /Users/braden/Projects/playwith-ideas && test -f bayes/index.html && python3 -m http.server 8000
```
