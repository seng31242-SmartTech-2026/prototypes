# UX Decisions — SmartTech

This document records the key UI/UX decisions made during the wireframing phase (SENG 31242, Weeks 5–7) for the Buyer, Seller, and Admin portals, with a brief rationale for each, per Course Guideline §7.1.1.

> Note: this is a starting draft based on the screens/components named in the sprint issues. Go through each section and adjust anything that doesn't match what's actually in the Figma files — I can't see the live designs myself, so this should be checked against them before committing.

---

## 1. Layout Strategy

**Buyer portal — mobile-first (375px), scaled up to desktop (1280px)**
Mobile optimisation is a stated UVP for SmartTech, so the buyer-facing flow (browsing, cart, checkout) is designed for the smaller viewport first, then expanded for desktop with extra breathing room for things like side-by-side product comparison or a wider filter panel.

**Admin / Seller portals — desktop-first**
Both personas (shop owner, seller) primarily manage inventory, orders, and analytics from a desktop, so these layouts prioritise information density (tables, multi-column dashboards) over mobile constraints.

**Low-fidelity, no colour**
Wireframes are intentionally greyscale at this stage so stakeholder feedback stays focused on layout, hierarchy, and flow rather than visual styling — consistent with how the SRS/SDS documents were kept black-and-white.

---

## 2. Navigation Structure

**Buyer portal:** persistent top nav (Home, Products, Cart, Account) on desktop; condensed to a bottom tab bar on mobile for one-handed thumb reach.

**Admin / Seller portals:** a left sidebar (Dashboard, Products, Inventory, Orders, Reports) that collapses to icons-only on narrower viewports, since both are desktop-first and benefit from the sidebar staying visible during long table/list sessions.

---

## 3. Key Component Conventions

**Compatibility Assistant widget (Product Detail page):** device-selection dropdown sits above a "compatible products" panel, kept visually distinct from the main spec block so it reads as a tool, not just another spec row.

**Specification filter panel (Product Listing page):** RAM / storage / brand / price-range filters grouped in a collapsible sidebar on desktop; on mobile this collapses into a "Filters" button that opens a bottom sheet, to avoid eating vertical space on a small screen.

**Order status workflow (Admin Order Management):** shown as a horizontal stepper — Pending → Confirmed → Shipped → Delivered — so the current stage is unambiguous at a glance.

**Low-stock alerts (Admin Inventory Management):** flagged with an icon + text label ("Low stock"), not colour alone, so the alert still reads correctly in a greyscale wireframe and stays accessible regardless of colour vision.

---

## 4. Accessibility Considerations

- Status indicators (low-stock badges, order stages) use icon + text, never colour as the only signal.
- Form fields (checkout address, payment, registration) use persistent visible labels rather than placeholder-only text, so the field purpose doesn't disappear once a user starts typing.
- Interactive elements sized for a minimum ~44×44px tap target on the mobile layouts.

---

## 5. Open Items

- [ ] Confirm breakpoints are applied consistently across all 8 buyer screens (some may need a pass to verify both 375px and 1280px versions exist).
- [ ] Confirm the above conventions actually match what's in the three Figma files — this draft was written from the issue descriptions, not the live designs.
- [ ] Add screen-by-screen notes if the team wants more granular rationale than the conventions above.