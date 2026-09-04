# vault-personal

Private-life knowledge for the Agent Context Engine, on a **personally-owned** GitHub
account.

## One of N vaults

This vault is not a special case. ACE hosts any number of vaults — `vault-spx`,
`vault-personal`, `vault-clientA` — all structurally identical, each declaring in its own
`vault.json` which classes of content it accepts. This one accepts `private-life`; a work
vault accepts `professional`. That is the only difference.

Nothing else in the system treats "personal" as a distinct kind of vault.

## Why this is a separate repository

Custody. An enterprise-managed account is readable by enterprise administrators and is
reclaimed at offboarding. Anything here would be content you no longer controlled.
Keeping it on a personal account means work knowledge can be backed up, shared, and
pushed freely without dragging private life along with it.

Git pushes history, not the working tree — so separation has to be by repository, not by
folder or by `.gitignore`.

## What belongs here

- `personal\` — your own profile, household, calendar, interests
- `people\` — rapport overlays: family, hobbies, birthdays, personal circumstances
- Personal reflection that is not work journalling

## What does not

- Anything about a working relationship — role, routing, projects, availability. That
  belongs to the vault that accepts `professional` for that employer or client, and
  duplicating it here creates drift.
- Protected-category data about colleagues. `protected` is an engine constant that **no**
  vault accepts. Moving such data out of an employer tenant reduces one exposure; it does
  not make holding it appropriate.
- Credentials, in any vault, ever.

## The overlay rule

A person may have a file in more than one vault, sharing the same **slug**:

```
vault-spx\people\jane-doe.md         identity + how to work with them
vault-personal\people\jane-doe.md    rapport only
```

**No fact appears in two files.** This one is an overlay, never a copy — so the records
cannot drift out of agreement. The professional record stays canonical for slug, name,
and role. Search merges them by slug at read time.

Full policy: `vault-spx\notes\topics\vault-knowledge-classification.md`.

## Default sensitivity

`private`. Nothing here is published anywhere.
