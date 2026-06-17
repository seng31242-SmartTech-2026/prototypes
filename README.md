# prototypes — SmartTech

This repository contains all **UI design artefacts** produced during the design phase of the SmartTech project (SENG 31242 – System Design Project, University of Kelaniya, 2026).

---

## Repository Purpose

The `prototypes` repository stores wireframes, user flow diagrams, Figma prototype links, and exported images. These artefacts translate the requirements captured in the SRS into tangible UI concepts, ready to inform the full Software Design Specification (SDS).

> ⚠️ **Design Phase Only:** This repository is active during Weeks 5–8 (System Design phase). No high-fidelity or coded prototypes should be committed here — those belong in the development phase (SENG 34213).

---

## Contents Structure

```
prototypes/
├── wireframes/
│   ├── links.md                 # Figma prototype links (source of truth)
│   └── exports/                 # PNG exports of each screen
│       ├── admin/
│       │   ├── admin-login.png
│       │   └── ...
│       ├── seller/
│       │   ├── seller-dashboard.png
│       │   └── ...
│       └── buyer/
│           ├── buyer-home.png
│           └── ...
│
└── decisions/
    └── ux-decisions.md          # UX rationale: layout choices, navigation, patterns used
```

---

## Figma Prototype Links

| Portal | Figma Prototype |
|---|---|
| Admin | https://www.figma.com/proto/2PUwTqXMKTU8wcFUwu8gfQ/Untitled?node-id=0-1 |
| Seller | https://www.figma.com/proto/MsUBp2qZsLwLGIAEKhFF6N/Untitled?node-id=0-1 |
| Buyer | https://www.figma.com/proto/ZzFxsdahB34cHOWMKhdgpd/Untitled?node-id=0-1 |

> Make sure each link has at least **view/comment access** turned on for the team and the marker, since this link is the editable source — there's no `.fig` file committed alongside it.

---

## Screens to Cover

The following screens must be wireframed as a minimum. Update the Status column as work progresses.

| Screen | Description | Status |
|---|---|---|
| Landing / Home | Public-facing page; shop discovery | ☐ |
| Shop Registration | New shop onboarding form (multi-step) | ☐ |
| Shop Dashboard | Owner's main management hub | ☐ |
| Service Request List | List and filter incoming service jobs | ☐ |
| Service Request Detail | View and update a single job | ☐ |
| Customer Portal | Public shop profile and service catalogue | ☐ |
| Login / Authentication | Sign-in, password reset flows | ☐ |
| Settings / Profile | Shop details, team management | ☐ |

Add additional screens as identified during the design review.

---

## Tooling Required

| File Type | Tool | Notes |
|---|---|---|
| Figma prototype link | [Figma](https://figma.com) | Source of truth — open directly via the links above |
| `.png` | Any image viewer | Static exports for offline review and grading |

---

## Note on Source Files

This repo does **not** commit editable `.fig` files. The Figma prototype links above are the editable source — anyone needing to edit the design opens the link directly in Figma. The `exports/` folder holds static PNG snapshots of each screen, committed alongside the links so the work is reviewable without a live Figma session.

---

## UX Decisions

All significant UI/UX decisions — choice of layout patterns, navigation structure, component conventions, accessibility considerations — must be documented in [`decisions/ux-decisions.md`](decisions/ux-decisions.md) with a brief rationale for each choice.

---

## Branching & Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full branching strategy and commit message convention used in this repository.

---

*© Software Engineering Teaching Unit, University of Kelaniya — SENG 31242, 2026*
