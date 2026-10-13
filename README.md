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

---

## Start with the journey

The plan opens on **the journey**, because that is the part worth arguing about
first. Eighteen stages, from an empty portal to a certified officer, grouped
into seven acts, with the four handovers marked — institute to cadet at
enrolment, institute to company at consent, company to ship at sign-on, and
ship back to institute at submission. Those handovers are where a portal like
this actually fails, because the baton is already with somebody who does not
work for the institute.

Everything else in the plan belongs to a stage in that journey.

## The eleven sections

1. **The journey** — 18 stages in seven acts; open any stage for what the system does, the records it creates, the decisions it enables, how it goes wrong, and what differs for an international candidate
2. **Overview** — the problem, the three surfaces, the design principles, and a coverage check against version 1
3. **Role surfaces** — what each audience can do, and the refusals that matter
4. **Permissions** — 61 objects against 11 roles
5. **Feature catalogue** — 203 features across 22 modules, filterable by phase, module, surface and priority
6. **Rule engines** — the 11 deterministic engines that make this more than a records system
7. **Data model** — 85 entities, the lifecycle state machines, the derived figures, and a full specification of what is captured about a cadet
8. **Decision register** — the 18 decisions the platform exists to support
9. **Build order** — nine phases, sequenced by dependency
10. **Technology** — the stack, the engineering rules, and how a phase closes
11. **Open questions** — what has to be answered before Phase 0 starts

---

## Status

This is a specification, not a codebase. It is written to be handed to a
developer and built against. Nothing in `index.html` is generated at runtime and
nothing is fetched from a network — the plan is the data and the data is in the
file.

The rules the product will be held to — what a company may see, what gets
logged, what can never be deleted — are deliberately **not** settled here yet.
The journey comes first; the constraints are a separate conversation once the
flow is agreed.

**Confidential.** ISF Group, Mumbai.
