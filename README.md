# vault-personal

Private-life knowledge for the Agent Context Engine, on a **personally-owned** GitHub
account. Deliberately separate from `vault-work`, which lives on employer-controlled
infrastructure.

## Why this is a separate repository

Custody. An enterprise-managed account is readable by enterprise administrators and is
reclaimed at offboarding. Anything here would be content you no longer controlled.
Keeping it on a personal account means work knowledge can be backed up, shared, and
pushed freely without dragging private life along with it.

Git pushes history, not the working tree — so separation has to be by repository, not
by folder or by `.gitignore`.

## What belongs here

- `personal\` — your own profile, household, calendar, interests
- `people\` — rapport overlays: family, hobbies, birthdays, personal circumstances
- Personal reflection that is not work journalling

## What does not

- Anything about the working relationship — role, routing, projects, availability.
  That is `vault-work`, and duplicating it here creates drift.
- Protected-category data about colleagues. Moving it out of the employer tenant
  reduces one exposure; it does not make holding it appropriate.
- Credentials, in any repository, ever.

## The overlay rule

A person may have a file in both roots, sharing the same **slug**:

```
vault-work\people\jane-doe.md        identity + how to work with them
vault-personal\people\jane-doe.md    rapport only
```

**No fact appears in both files.** This one is an overlay, never a copy — so the two
cannot drift out of agreement. The work file stays canonical for slug, name, and role.

Full policy: `vault-work\notes\topics\vault-knowledge-classification.md`.

## Default sensitivity

`private`. Nothing here is published anywhere.
