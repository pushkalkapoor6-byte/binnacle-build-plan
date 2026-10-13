# Binnacle — build plan

**Placement and sea service, for the institute.**

A placement and sea-service management portal for DG Shipping-approved maritime
training institutes in India. One record of a cadet that runs from the first
enquiry to the Certificate of Competency, with three audiences looking at it
through three different windows: the **institute** that owns the record, the
**company** that is shown a consented slice of it, and the **cadet** who
controls which slice that is.

---

## What is in here

| File | What it is |
| --- | --- |
| `index.html` | The build plan. A single self-contained page — open it in any browser, no server and no build step. |

The plan has twelve sections, navigable from the rail on the left:

1. **Overview** — the problem, the three surfaces, the design principles, and a coverage check against the original scope
2. **Non-negotiables** — the thirteen rules that cannot be traded away, four of them legal positions
3. **The journey** — 17 stages, from an empty portal to a certified officer; open any stage for what the system does, the records it creates, the decisions it enables and how it goes wrong
4. **Role surfaces** — what each audience can do, and the refusals that matter
5. **Permissions** — 61 objects against 11 roles
6. **Feature catalogue** — 203 features across 22 modules, filterable by phase, module, surface and priority
7. **Rule engines** — the 11 deterministic engines that make this more than a records system
8. **Data model** — 85 entities, the lifecycle state machines, the derived figures, and a full specification of what is captured about a cadet
9. **Decision register** — the 18 decisions the platform exists to support
10. **Build order** — nine phases, sequenced by dependency
11. **Technology** — the stack, the engineering rules, and how a phase closes
12. **Open questions** — what has to be answered before Phase 0 starts

---

## The four that decide whether this is lawful

Read section 02 before anything else. In short:

- **Nothing is ever charged to a cadet for a placement.** Maritime Labour
  Convention 2006, Regulation 1.4. Course fees are the institute's own business
  and are handled separately. The placement side of the schema carries no
  monetary field at all, so the statutory register of fees charged to cadets
  stands at nil by construction.
- **No artificial intelligence anywhere.** Every figure is arithmetic over rows
  a person can reproduce by hand.
- **A company sees a slice, never the house.** No disclosure without live
  consent; contact details never before an accepted request; welfare and
  disciplinary detail disclosable to nobody. No role overrides this.
- **Every write and every read is logged**, append-only, including who looked at
  a cadet's file.

---

## Status

This is a specification, not a codebase. It is written to be handed to a
developer and built against. Nothing in `index.html` is generated at runtime
and nothing is fetched from a network — the plan is the data and the data is in
the file.

**Confidential.** ISF Group, Mumbai.
