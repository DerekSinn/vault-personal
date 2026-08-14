---
type: reference
title: Profile — Derek Sinn
date: 2026-08-14
tags: [profile, personal, identity, working-style]
engagements: []
projects: []
people: []
source:
sensitivity: private
status: draft
summary: "Who Derek is, how he thinks, and what he is working toward — the context an agent needs to be a colleague rather than a stranger with filesystem access. Distinct from memory\\user.md, which holds discrete preferences; this holds the standing picture."
---

# Profile — Derek Sinn

## What this file is, and why it is not `memory\user.md`

`memory\user.md` holds **discrete rules**: "use `pwsh`, not `powershell`", "never run SQL
without approval." Each is a small, independently-checkable fact with its own provenance.

This file holds the **standing picture** — background, how he reasons, what he is trying to
build, what a normal day looks like. It is not decomposable into rules, and it is what makes
the difference between an agent that follows instructions correctly and one that anticipates
what the instruction was *for*.

Both are needed. Neither substitutes for the other.

## Write policy

**This matters more than the content**, because a profile an agent may silently rewrite is a
profile that drifts into whatever the agent last inferred.

| Section | May an agent update it? |
|---|---|
| **Who I Am** | **No.** Derek's alone. |
| **What I Want** | **No.** Derek's alone. Goals stated by him, not inferred from activity. |
| Background | Only from something he said, quoted or paraphrased closely. |
| How I Think | Yes, additively, with provenance. |
| Daily Routine | Yes, additively, with provenance. |
| Interests & Context | Yes, additively, with provenance. |

Rules for the sections an agent may touch:

- **Add, never overwrite.** If a new observation contradicts an existing line, leave both and
  flag the contradiction — a person's habits genuinely change, and a silent overwrite
  destroys the evidence that they did.
- **Provenance is mandatory**, same `<sub>` format as `memory\`:
  `<sub>added YYYY-MM-DD · confidence: verified|stated|inferred · source: <where></sub>`
- **`inferred` is the weakest grade and the first to re-check.** One session's guess about
  how someone thinks, left unmarked, becomes next year's settled fact.
- **Log every update** on the *Profile Updates* line of that day's journal entry, so a day's
  changes to this file are visible in one place without diffing it.
- **Never write anything here that he has not seen.** He should be able to read this file and
  recognise himself. If a line would surprise him, it does not belong.

---

## Who I Am

<!-- Derek's alone. Agents: do not fill this in. -->

*Not yet written.*

## Background

*Not yet written.*

## How I Think

*Not yet written — this section accretes from observation, with provenance on every line.*

## What I Want

<!-- Derek's alone. Goals as he states them, not as inferred from what he works on. -->

*Not yet written.*

## Daily Routine

*Not yet written.*

## Interests & Context

*Not yet written.*

---

## Provenance

Created 2026-08-14 as part of porting the "living profile" idea from `ai-memory-vault`. The
write policy was designed first and deliberately: the original had named sections an agent
could silently update, but no provenance and no audit trail, so there was no way to tell a
recorded fact from an accumulated guess. Ours carries the `memory\` provenance format and a
journal log line, which makes "silent" updates auditable after the fact.

Deliberately left empty rather than seeded from inference. A profile written *about* someone
by an agent, from observed behaviour, is exactly the artefact that reads plausibly and is
wrong in ways nobody notices. It gets filled by interview.
