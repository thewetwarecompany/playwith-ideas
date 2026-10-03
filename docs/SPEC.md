# Spec — Playwith.ideas

What the library does, part by part. Each part has a "Done when" test a person can check by hand. Parts marked **Not decided** wait on an open question in `docs/DECISIONS.md`; nobody builds them until Braden settles it.

## 1. An explorable page

One page teaches one idea. The reader acts first and the idea is named after. The order is: hook, play, reveal, name the concept, where it shows up in life. Any formula comes last and uses the colours and objects the reader already touched.

**Done when** all of these hold, checked by opening the page in a browser:
- It lives at `name/index.html`, with its CSS and JavaScript inside that one file. Fonts or images, if any, sit in the same folder.
- It works and reads well at 360 pixels wide and at desktop width.
- The folder weighs under 500 KB in total, fonts included.
- With the network switched off after loading, it keeps working.
- Every control can be reached and used with the keyboard alone, and the focus is visible.
- Numbers that change as you play are announced to a screen reader (`aria-live`).
- With reduced motion switched on in the operating system, nothing animates.
- No meaning is carried by colour alone: shape, outline or a label carries it too.
- Setting each control to its lowest and highest value breaks neither the numbers nor the sentences.
- The browser console shows no errors, and the network panel shows no tracker or analytics request.
- With JavaScript off, a reader can tell what the page would have shown.

Source: founding `CONTRIBUTING.md`, 2026-08-22.

## 2. The Bayes page, *The Test Says Yes*

1,000 dots stand for people. Three sliders set how many have a condition, how often the test catches it, and how often it flags a healthy person. A button hides everyone who tested negative. A sentence and a bar update as you play, and three preset buttons jump to a rare disease, a common flu and a nearly perfect test.

State: built on 2026-08-22 in the founding chat. Not in this repository.

**Done when:**
- It is in this repository at `bayes/index.html`.
- The sliders run from 1 to 200 people in 1,000, from 50 to 100 per cent, and from 0 to 20 per cent.
- At the starting values (10 in 1,000, 90 per cent, 9 per cent) the sentence says 98 people are flagged, 9 of them are truly sick, and a positive result means a 9 per cent chance.
- Pressing "Show only the positives" fades every dot without a ring, and pressing it again brings them back.
- It passes every check in part 1.

## 3. Letters

Each working session leaves a numbered letter in `letters/`: what was done, what was learned that is not written elsewhere, what should come next.

State: the first letter, `000-day-one.md`, exists in the founding chat. Not in this repository.

**Done when:**
- `letters/000-day-one.md` is in the repository.
- Every commit that changes a page also adds a letter with the next number.
- No earlier letter has been edited; the commit history shows each letter added once.

## 4. The index page — Not decided

A static page listing every explorable with its title and one line. The founding documents say a static index is enough and a search backend is not wanted. Its design and words have not been written.

**Done when:** opening the site's root shows every folder that holds a page, each linking to it, and passing the checks in part 1 that apply to a page with no controls.

## 5. Further pages — Not decided

Proposed in the founding letter, in this order: flocking (nudge one bird and the flock breaks), compound growth (how late the curve turns upward), and attention in language models (flagged there as at risk of dating badly). None is approved.

**Done when**, for each page Braden approves: it passes every check in part 1, and the reviewer can name the moment of surprise in one sentence.

## 6. Hosting and deploying — Not decided

Waits on Q-04 (which host) and Q-03 (which name and address). The founding documents say deploying is a merge to `main`, with no step that can fail between.

**Done when:** after a merge to `main`, the changed page answers at the public address within the time the host states, and `curl -sS -I` on that address prints `HTTP/2 200`.

## 7. Licence — Not decided

Waits on Q-02.

**Done when:** a `LICENSE` file is in the repository root and every page's footer names the same licence.

## 8. Contributions — Not decided

The founding `CONTRIBUTING.md` proposes that anyone proposes a page in a GitHub issue answering four questions (the idea in one sentence, the moment of surprise, the interaction in one sentence, why it will still be true in ten years) and waits for approval before building. An AI contributor says so and names the human sponsoring the merge. Whether this repository accepts outside contributions has not been decided.

**Done when:** a contributing guide is in the repository and its process has been used once, end to end.

## 9. Money — Not decided

Today there is no money, no treasury and no donation link. The founding documents allow, in order, a quiet sponsor link (Open Collective preferred, because its ledger is public), grants, and a person funding a named page who is credited in its footer and gets no editorial say. Any of these is bound by charter rule 5.

**Done when:** not applicable until Braden decides to take money. Then: the ledger is public, and the repository records who co-signs.
