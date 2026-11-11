# CANON — appbrewco/.github canonical map

The org's public defaults home: community-health files, the org
profile, and the workflow starter templates. Runtime automation is not
canon here — the live reusable workflows, the seed flow, the
governance skill, and the agent registry live in the org's private
runtime repository. This map is where a change starts (Maintainer
Contract rule 1: search before write).

## Entries

- `profile/README.md` — the org profile: the landing page at
  github.com/appbrewco, describing the org's public, static defaults.
- `ISSUE_TEMPLATE/` — the issue forms (`agent-task.yml`,
  `bug-ci-failure.yml`) and `config.yml` (blank issues disabled;
  contact links route security reports to the private channel).
- `PULL_REQUEST_TEMPLATE.md` — the org-wide pull request description
  template every PR in the org starts from.
- `SECURITY.md` — the security policy: supported versions, how to
  report vulnerabilities, response expectations.
- `workflow-templates/` — the starter workflows offered in the org's
  "new workflow" picker, each with its `.properties.json` manifest;
  the starters point at the private runtime repository's reusable
  workflows.
- `AGENTS.md` — the disclosure rules for this public repo (what may
  and may not be written here) plus the Maintainer Contract stub.
- `.editorconfig` — the formatting contract for files in this repo.

## Neighbors (never forked here)

- The org's private runtime repository — the live reusable workflows,
  the seed flow, the governance skill, the agent registry. Public
  repos run no org automation.
