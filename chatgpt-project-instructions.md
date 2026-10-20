# BlueBubbles Server: ChatGPT project instructions

## Roles and sources
- Project: `syuu1228/bluebubbles-server`, forked from `BlueBubblesApp/bluebubbles-server`. Helper is a separate repository, not part of an ordinary Server task.
- This file guides ChatGPT research and task preparation; `AGENTS.md` guides Codex implementation. Avoid duplicating its rules.
- Standing instructions must not embed an active upstream version, branch, tag, patch list, target OS, Private API/SIP configuration, runner, or release procedure. Resolve them from current user decisions, approved release-specific design/patch ledger, and current repository state.
- Separate user decisions, proposals, verified facts, assumptions, and obsolete plans. Inspect current code and relevant documents; if critical context is unavailable, mark it unverified rather than guessing.
- When upstream releases change, reassess fix inclusion without silently changing the selected work baseline.

## Backport preparation
- For each proposed fix, establish upstream inclusion, issue/PR and source patch evidence, impacted code, dependencies, adopted/excluded portions, risks, and regression checks.
- Record version-specific decisions and acceptance criteria in the approved design and patch ledger, not these instructions. Do not delegate implementation until necessary selection decisions and authorization are resolved.
- Avoid broad merges and unrelated changes merely to obtain fixes. Stay within the approved scope; do not require separate approval at every internal stage unless requested.
- Do not promote unverified issue reports, old assistant proposals, or obsolete plans into approved requirements.

## Preparing Codex work
- Inspect only relevant current code/tests, `AGENTS.md`, approved design/ledger, and primary patch evidence. Pass decisions and concrete acceptance tests to Codex, not raw research or repeated policies.
- Write concise task instructions (Goal, Scope, relevant Constraints, Verify, Commits), identifying the repository/ref and expected result. Require coherent commits and accurate verification reporting.
- When using task or audit tooling, consult its current documentation and validate the instruction format; do not import tool-specific conventions from other repositories.
- Treat changes to standing instructions or safety policies as separately authorized work, not incidental patch cleanup.

## Verification and reporting
- Follow the approved release-specific design and actual CI workflow for packaging, publication, release notes, signing, and rollback.
- Distinguish source/CI checks from macOS target-host validation. For Messages, Contacts, Apple Events, permissions, and client interoperability, specify what was actually tested.
- Report performed actions, commit SHAs, checks, limitations, and unresolved matters. Never claim a build, push, release, or target-host test occurred without evidence.
