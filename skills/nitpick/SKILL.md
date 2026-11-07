---
name: nitpick
description: Ruthless, ranked critique of any work before it ships (video, post, doc, deck, landing page, code, plan). Looks at the real thing, ranks problems by damage, and picks the fixes worth making. Use when someone says /nitpick, nitpick this, tear this apart, roast this, or what's wrong with this.
---

# /nitpick

Find what is wrong with a piece of work before the audience does. The output is a ranked list of problems and a recommended fix set, not a rewrite. Do not change the work unless asked.

Usage: `/nitpick [target] [--for <audience or goal>] [--depth quick|full]`
- No target: nitpick the most recent deliverable in the conversation.
- `--for`: who it is for and what it must achieve (e.g. "launch post, strangers scrolling on a phone"). If missing, infer it from context and state the assumption in one line.
- `--depth quick`: top 5 only. Default `full`.

## 1. Look at the real thing

Never critique from memory or from the plan. Open the actual artifact the way the audience will meet it:
- Video: pull stills from every scene and from mid-transitions; check the first 2 seconds and the last frame; view it at phone size.
- Page or app: screenshot it at desktop and phone width, light and dark.
- Doc, post or deck: read it top to bottom as a stranger, then only the headings and first lines as a skimmer.
- Code: read the diff and run it or its tests if you can.
- Plan: check it against the stated goal and constraints.

If something is not finished yet, critique what exists plus the plan, and say which parts were judged from the plan.

## 2. Hunt

Run each lens. Skip any that do not apply.
1. **Promise vs proof**: every claim, benefit or number. Is it shown or backed, or only stated? Do numbers match what is on screen or in the data?
2. **Clear to a stranger**: after one pass, does someone new know what it is, who it is for, why they should care, and what to do next?
3. **Hook and ending**: the first 2 seconds or first line; the final frame or call to action.
4. **Repetition and gaps**: the same thing shown twice; something important never shown.
5. **Trust killers**: placeholder text, "Example" or "Lorem" labels, mismatched numbers, broken links, stale facts, anything that reads as fake.
6. **Legibility**: text too small for the real viewing size, low contrast, collisions, clutter, text on screen too briefly to read.
7. **Voice and copy**: vague or clunky lines, generic phrasing ("streamline your workflow"), AI-writing tells (not-X-but-Y framing, em dashes, one-line closers, forced triads, inflated significance), violations of the house style if one exists.
8. **Craft**: pacing, sound, transitions, consistency. For code: errors, edge cases, security, performance.
9. **Privacy and safety**: personal data, secrets, real names, anything that should not go public.

Be specific. Name the scene, timestamp, line, file or element, and say what the audience actually experiences. "Caption covers the Focus 1 label at 0:33" beats "some overlap".

## 3. Rank

Group findings by damage, worst first, numbered continuously:
- **Hurts the message**: the audience misses the point, or the core claim is unproven.
- **Weakens trust**: the audience starts to doubt it.
- **Polish**: noticeable, not fatal.

Each item: a bold short label, then one or two sentences with the evidence and a concrete fix. No item without a fix. Cap at about 12; drop trivia rather than pad.

## 4. Pick

- Open with the single biggest problem in one sentence, plus a confidence score from 1 to 5 and what would change your mind.
- End with **My pick**: which item numbers to fix now, which to skip, what fixing costs (time, rework, re-render) and any cheaper alternative.
- Last line: one next action the user can answer in a word or two.

## Rules

- Honest over nice. Do not soften real problems, and do not invent problems to look thorough.
- Praise only when it changes a decision ("keep the hook, it works").
- Never fix, rewrite, re-render or publish as part of a nitpick. Offer it.
- Keep it scannable: bold labels, short lines, no walls of text.
