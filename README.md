# prototypes — SmartTech

This repository contains all **UI design artefacts** produced during the design phase of the SmartTech project (SENG 31242 – System Design Project, University of Kelaniya, 2026).

---

## Repository Purpose

The `prototypes` repository stores wireframes, user flow diagrams, Figma exports, and low-fidelity prototypes. These artefacts translate the requirements captured in the SRS into tangible UI concepts, ready to inform the full Software Design Specification (SDS).

> ⚠️ **Design Phase Only:** This repository is active during Weeks 5–8 (System Design phase). No high-fidelity or coded prototypes should be committed here — those belong in the development phase (SENG 34213).

---

## Contents Structure

```
prototypes/
├── wireframes/
│   ├── source/                         # Editable source files
│   │   ├── shop-registration.fig       # Figma source (if exported)
│   │   ├── shop-dashboard.drawio       # draw.io source
│   │   └── ...
│   └── exports/                        # PNG or PDF exports of each screen
│       ├── shop-registration.png
│       ├── shop-dashboard.png
│       └── ...
│
├── user-flows/
│   ├── flow-shop-onboarding.drawio     # User flow source
│   ├── flow-service-request.drawio
│   └── exports/
│       ├── flow-shop-onboarding.svg
│       └── flow-service-request.svg
│
└── decisions/
    └── ux-decisions.md                 # UX rationale: layout choices, navigation, patterns used
```

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
| `.fig` | [Figma](https://figma.com) | University email may qualify for free Education plan |
| `.drawio` | [draw.io / diagrams.net](https://app.diagrams.net/) | Free, browser-based |
| `.png` / `.pdf` | Any image or PDF viewer | For reviewing exported wireframes |

> ⚠️ **Source File Rule:** Both the editable source file **and** the exported image must be committed. Committing only a PNG is not acceptable — team members must be able to open and edit the source.

---

## UX Decisions

All significant UI/UX decisions — choice of layout patterns, navigation structure, component conventions, accessibility considerations — must be documented in [`decisions/ux-decisions.md`](decisions/ux-decisions.md) with a brief rationale for each choice.

---

## Branching & Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full branching strategy and commit message convention used in this repository.

---

*© Software Engineering Teaching Unit, University of Kelaniya — SENG 31242, 2026*
