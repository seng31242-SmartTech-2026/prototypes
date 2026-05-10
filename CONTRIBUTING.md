# Contributing to `prototypes`

This guide defines the branching strategy and commit conventions for the `prototypes` repository. All team members must follow these rules before making any contribution.

---

## Branching Strategy

| Branch Pattern | Purpose | Example |
|---|---|---|
| `main` | Latest approved, reviewed work. Merges via PR only. | `main` |
| `draft/<screen-or-flow>` | Active working branch for a screen or user flow in progress. | `draft/shop-dashboard-wireframe` |
| `fix/<issue-number>` | Corrective changes addressing design review feedback. | `fix/29` |

**Rules:**
- Never commit directly to `main`.
- Branch off the latest `main` when starting new work.
- Delete your branch after it is merged.

```bash
git checkout main
git pull origin main
git checkout -b draft/service-request-wireframe
```

---

## Commit Message Convention

Follow the **Conventional Commits** specification adapted for a UI/prototype repository.

```
<type>(<scope>): <short imperative summary>

[Optional body: explain WHY, not WHAT]

[Optional footer: Closes #<issue-number>]
```

### Allowed Types

| Type | When to Use |
|---|---|
| `feat` | Adding a new wireframe, user flow, or screen |
| `fix` | Correcting a wireframe based on design review or supervisor feedback |
| `refactor` | Restructuring layouts or flows without changing the design intent |
| `docs` | Updating UX decision notes or README |
| `chore` | Repository housekeeping (folder structure, .gitignore, README) |
| `style` | Visual-only adjustments (spacing, colour, label corrections) |

### Allowed Scopes

`wireframes` · `user-flows` · `ux-decisions` · `exports` · `readme`

### Good Examples ✅

```
feat(wireframes): add low-fidelity wireframe for shop registration screen

Covers 3-step onboarding: business details, services, confirmation.
Source: wireframes/source/shop-registration.drawio
Export: wireframes/exports/shop-registration.png

Closes #34
```

```
fix(wireframes): update dashboard navigation based on design review feedback

Moved "Service Requests" to primary nav per reviewer comment on PR #41.
Refs #29
```

```
docs(ux-decisions): document navigation pattern rationale

Chose tab-based navigation over sidebar for mobile-first responsiveness.
```

### Bad Examples ❌

```
new wireframe / updated design / fix / v2 / final design
```

---

## Source File Requirement

Every wireframe or flow committed must include **both**:

| What | Where |
|---|---|
| Editable source file (`.drawio`, `.fig`) | `wireframes/source/` or `user-flows/` |
| Exported image (`.png` or `.svg`) | `wireframes/exports/` or `user-flows/exports/` |

Committing only an exported image is **not acceptable**. Teammates must be able to open and edit the source.

---

## Pull Request Checklist

Before marking a PR as Ready for Review, confirm:

- [ ] Both source file and export are committed
- [ ] Screen/flow is listed in the README screens table and status updated
- [ ] Wireframe is low-fidelity (no colours, no final copy — boxes and labels only)
- [ ] Any significant UX decision is documented in `decisions/ux-decisions.md`
- [ ] No spelling errors in labels or annotations
- [ ] PR description links to the related GitHub Issue (`Closes #N`)
- [ ] At least one team member is assigned as reviewer

---

*© Software Engineering Teaching Unit, University of Kelaniya — SENG 31242, 2026*
