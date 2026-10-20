# BlueBubbles Server agent rules

## Scope
- Work only on the authorized task. Inspect relevant code, tests, and upstream patches; avoid unrelated refactors, formatting churn, dependency upgrades, and wholesale merges.
- For backports, compare the selected baseline with the source fix, identify missing or partial changes, and retain issue/PR/commit provenance.
- Preserve client/API compatibility and application identity except where a reviewed fix requires otherwise. Do not modify product versions or runtime code merely to display backport metadata.

## Safety
- Do not change SIP, bypass TCC, enable Private API, or modify a separate Helper repository without authorization. Standard macOS permission grants are not TCC bypasses.
- Never write directly to live Messages databases, send real messages, change production settings, or install on production hosts without authorization.
- Do not expose or commit secrets, messages, contacts, signing material, or sensitive logs.

## Verification
- Add focused regression coverage where useful; run relevant checks and disclose failures or skipped tests.
- Review `git diff` and `git status --short`. Exclude unrelated, generated, and sensitive files; commit authorized work coherently unless told otherwise.
- Create or push release tags, or publish releases, only through an authorized release workflow after its completion criteria are met; never during ordinary implementation.
