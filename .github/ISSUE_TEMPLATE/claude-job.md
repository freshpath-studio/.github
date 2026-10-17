---
name: Claude job
about: A job for Claude via the Mac relay (add agent:claude when ready). Mac-only and TestFlight steps go at the top.
title: "<PM>-JOB: "
labels: []
---

## ⚠️ Mac-only / Apple / device steps (fill in FIRST, or write "None")
<!-- Claude (headless relay) can build, test and use the per-job simulator on the Mac mini. It can NOT:
     upload to TestFlight / App Store Connect (Cassie only, separate issue), click developer.apple.com, or use a physical iPhone. -->
- [ ] Needs the Mac mini (Xcode build, simulator, archive, local .ipa)? → label `needs-mac` — **yes / no**
- [ ] **TestFlight / App Store Connect upload is NEVER part of this job** (Daniel, Oct 16 2026). Cassie (AppStoreConnect) owns every upload. Stop at the version-bump PR. After it merges, the PM opens a separate "Cassie TestFlight handoff" issue labeled `needs-mac` + `needs-cassie` (and `bot:cassie` if the repo has that label). Does this job end in a build Cassie will upload? — **yes / no**
- [ ] Needs developer.apple.com screens (App IDs, capabilities, iCloud)? → `needs-cassie` — **yes / no**
- [ ] Needs a physical iPhone or Daniel's decision? → `needs-daniel` — **yes / no**
- [ ] Any money, sign-up, or public text (store copy, posts)? → stop: CFO / Legal first — **yes / no**

## Goal
<!-- One item, one small PR. What should be true when this is done? -->

## Acceptance checks
- [ ] 
- [ ] Tests / lint pass (`sh scripts/test.sh` or the repo's checks)

## Context
<!-- Spec section in docs/handoff/<App>-HANDOFF.md, related issues/PRs, screenshots. -->

## Out of scope
<!-- What Claude must not touch. -->

<!-- Reviewing Claude's result? If changes are needed: post ONE "<PM>-RESULT: Changes needed" comment on THIS issue
     with the full numbered fix list AND re-add agent:claude in the same step. -->
