---
name: detolstify
description: Compress a document, note, or session artifact down to what a reader actually needs — cutting ceremony, restatement, and connective tissue while keeping every specific intact. Use whenever the user says "detolstify", or asks to trim, tighten, shorten, condense, or cut the fluff from a doc, README, plan, spec, handoff note, or summary. Named for Lev Tolstoy, who wrote magnificent novels at enormous length. This skill removes the length, not the magnificence.
---

# Detolstify

**Compress by deletion, not by abstraction.** Replacing three specific sentences with one vague one is not compression — it's information loss disguised as brevity. The goal is fewer words carrying the same freight, never the same words carrying less. When in doubt, cut the connective and keep the specific.

## Pass 1 — Triage

Go sentence by sentence and sort each into one of three buckets.

**Load-bearing.** Numbers, names, paths, commands, versions, decisions and who made them, constraints, gotchas, open questions, anything that was expensive to learn. Test: if this vanished, would a reader do the wrong thing, or have to go ask someone? If yes, it stays.

**Scaffold.** Navigation and connective tissue: "in this section we'll cover", restatements of the request, recaps of what was just said, transitions, headers sitting over a single paragraph.

**Decoration.** Ceremony and padding: "it's important to note", "comprehensive", "robust", "very", "overall", hedges that hedge nothing, and closing summaries that repeat the body.

## Pass 2 — Cut

Delete all decoration. Delete scaffold unless the document is long enough that a reader needs to navigate it — under roughly a screen, no one is navigating.

Then dedupe: when the same fact appears in the intro, the body, and the summary, keep the instance closest to where it's used and drop the rest. Then look for format shifts, which beat wordsmithing every time:

- A paragraph enumerating options → a list
- Repeated parallel prose → a table
- The narrative of how you reached a conclusion → the conclusion, plus one line of why, plus the alternatives you rejected and the reason

## Pass 3 — Read it cold

Reread as someone who wasn't in the session. Every pronoun must have a visible referent, every step its precondition, every term its first definition. Concise is not cryptic — if a reader has to reconstruct what you removed, put it back.

## Never cut

Code, commands, config, data, quotes, and error messages stay verbatim. Do not paraphrase an error message; the exact string is the thing that's searchable.

## Stop condition

Stop when the next cut would remove information rather than words. There is no target length — length is earned, sentence by sentence, and a document that earns 2000 words keeps them.

## Report

Close with one line: what classes of thing you cut, and the before → after word count. Separately flag any cut that was a judgement call, so the user can veto it without rereading the original.

If the text carries weight you can't assess — contractual language, a spec others are building against, anything legal or regulatory — say so and stop rather than guessing at what's load-bearing.
