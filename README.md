# accountable-engine

**An accountability substrate for AI-era engineering — where evidence, not feeling, is the measure of the work and the worker.**

> Status: reference framework + working tooling. Proof-before-trust — what's here is what runs; anything aspirational is marked.
> Author: Zain Dana Harper ([HarperZ9](https://github.com/HarperZ9)). Published for provenance and priority — see [LICENSE](LICENSE).

---

## The problem

Two failure modes run the field, and they're usually the same person:

- **Crippling self-criticism** — the engineer who can't ship because every flaw reads as a verdict on their worth.
- **Godlike certainty** — the same engineer, hours later, sure everyone else's code is garbage.

They aren't opposites. They're one wound: **identity fused to the work.** When the work is good, the fusion reads as ego; when it falls short, as collapse. God one minute, nothing the next — same circuit, different input. "Just be more confident / more humble" fails because it tunes the *output* of a circuit whose flaw is the fusion itself.

The same problem, scaled, blocks multi-agent development: agents and people coordinate on *vibes* — "looks done," "should work," "I'm sure" — and the work drifts, because nothing external holds the line.

## The thesis

**Make evidence the measure instead of feeling — and aim it in both directions.**

Receipts are indifferent. A red build doesn't flatter the god or wound the collapse; it reports what the artifact does. The move underneath is one rule, applied to the human and the machine alike:

> **Awareness is not authority. The gate judges the action — never the worth of whoever took it.**

De-fuse identity from work, and both pathologies starve at once. Not two fixes. One cut.

## The mechanism: a bilateral substrate

It faces two directions.

**Inward — it judges the work.** Every claim of "done" must carry a *receipt*: a build result, a test count, a verdict — never an assertion. State is recorded, not narrated. The criticism is real but depersonalized — the build is red, not "you failed."

**Outward — it interrogates the operator.** A critic, generated from live state, asks the questions the gaps imply — *what finishes before you start something new? are you trusting that on a receipt or a vibe? is this in scope, or a relapse?* — and records the answers as decision-receipts. There is no flag to make it flatter you; its authority comes from reality, not preference.

Together they pull both poles to center. The self-critic ignores the green; the grandiose ignores the red; the substrate makes both look at the actual state. It is the regulator the psychology can't be — and, over repetition, a *trainer*: exposure to receipts recalibrates the self-model toward reality.

## What's here

- **[`STATE.template.md`](STATE.template.md)** — the coordination protocol: read → claim → isolate → receipt → record. A claim ledger so parallel agents don't collide; an append-only ledger of what shipped, with receipts; explicit bounds.
- **[`critic.ps1`](critic.ps1)** — the bilateral critic (reference implementation): reads live state and puts **FINISH / FOCUS / VERIFY / SCOPE** to the operator; `-Record` appends a decision-receipt to `DECISIONS.md`. Generated from state, not a question bank. (PowerShell reference impl; a portable port is open work.)

## Provenance

This repository stakes priority on the invention above — the bilateral, evidence-over-ego accountability substrate and its operator-facing critic — authored by Zain Dana Harper. The git history is the timestamped record.
