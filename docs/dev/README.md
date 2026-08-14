---
commissioned-by: spacedock@0.26.0
entity-type: task
entity-label: task
entity-label-plural: tasks
id-style: sd-b32
state: .spacedock-state
trunk: main
stages:
  defaults:
    worktree: false
    concurrency: 1
  states:
    - name: inbox
      initial: true
      gate: true
    - name: building
      worktree: true
    - name: checking
      gate: true
    - name: released
      terminal: true
---

# Synthetic Development Workflow

This commissioned workflow exists only for the disposable public projection
proof. Its custom stages deliberately avoid kc-dev-flow field assumptions.
