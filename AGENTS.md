# AGENTS.md — appbrewco/.github

This repository is the org's PUBLIC defaults home: community-health
defaults (issue/PR templates, SECURITY.md), the org profile, and the
`workflow-templates/` starter UI. It hosts **no runtime automation** —
the live reusable workflows, the seed flow, the governance skill, and
the agent registry live in the org's PRIVATE runtime repository
(callable from private org repos only; public repos run no org
automation and are hand-merged). The starter templates here point at
those private workflows for private repos to adopt.

Everything here — issues, PR descriptions and comments, commit
messages, release notes, workflow comments, file contents — is visible to
anyone on the internet and indexed by search engines and third-party
mirrors within minutes.

## Disclosure rules for agents (and humans)

Never write org-internal detail into this repo. That includes, without
limitation:

- Authentication architecture: GitHub App names/IDs, token scopes and
  minting flows, secret names, credential-rotation plans.
- Internal repo inventories, dependency graphs between private repos, or
  named private packages.
- Operational practice: runner topology, deployment processes, failure
  post-mortems, migration playbooks, who/what merges when.
- Anything that exists only to coordinate work inside the org.

If a task needs that context to be written down, put it in a private repo,
a local file, or the issue tracker of a private repository — not here.
When linking from this repo to internal context, link to a private
resource (readers without access will simply see a 404) instead of
inlining the content.

Cross-repo migration/tracking issues that list org repos and their CI
states belong in a private ops repo. Issue and PR *comments* can be
hard-deleted; edited *bodies* keep public revision history, and commit
messages are effectively permanent — assume anything written here is
irreversible.

CI workflow YAML necessarily encodes some structure (job names, action
references); that is accepted. Prose descriptions around it are where
leaks happen — describe *what the workflow does*, never *how the org is
organized*.

---

<!-- BEGIN MAINTAINER CONTRACT STUB (synced verbatim from the gh-appbrew kit: skills/gh-appbrew/references/contract-stub.md; fix the canonical and re-sync, never edit here) -->
Canonical body: gh-appbrew `skills/gh-appbrew/references/maintainability.md` (do not edit
this stub locally; fix the canonical and re-sync).

1. Search before write — check the repo and its CANON map first; use or extend the canonical, never fork it.
2. Delete what you obsolete — superseding code deletes its predecessor in the same PR; git history is the archive.
3. Docs are present tense — no dates/rulings; history lives in CHANGELOG.md, incidents in postmortems/.
4. Same-PR parity — behavior changes ship with their doc + test updates, or the PR is incomplete.
5. Prefer removal to addition, editing a file to adding a file, generated docs to prose restating code.
6. Patches don't stack — fixes land on the origin file/branch; the third patch on the same spot requires a refactor proposal.
7. Net accounting — every PR states added/removed/justification (or "nothing to delete").
8. No commented-out code, dead flags, temp files, or docs describing things that no longer exist.
9. Agents are maintainers of record, not visitors — leave it simpler, or say why in the PR.
10. If your change invalidates a doc/skill/rule, fixing that is in scope.
<!-- END MAINTAINER CONTRACT STUB -->
