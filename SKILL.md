---
name: handoff
description: Compact the current conversation into a handoff document for another
  agent to pick up.
argument-hint: What will the next session be used for?
disable-model-invocation: true
license: MIT
metadata:
  author: Matt Pocock
  adapted_by: Igor Guariroba
  version: 1.0.0
---


Write a handoff document summarising the current conversation so a fresh agent can continue the work. Save to the temporary directory of the user's OS (`$TMPDIR`, else `/tmp`; `%TEMP%` on Windows) - not the current workspace.

Include a "suggested skills" section with each skill's name, absolute `SKILL.md` path and the condition for reading it. The next Pi agent loads those instructions through file reads; the user can also invoke an installed skill explicitly with `/skill:name`.

Do not duplicate content already captured in other artifacts (specs, plans, ADRs, issues, commits, diffs). Reference them by path or URL instead.

Redact any sensitive information, such as API keys, passwords, or personally identifiable information.

If the user passed arguments, treat them as a description of what the next session will focus on and tailor the doc accordingly.
