# Unified API Hub (Phase 1 Prototype)

▶ [View the live prototype](https://snwl-wchen.github.io/API-Hub-Phase1/)

A working MVP Phase 1 prototype for a unified developer portal, designed to consolidate SonicWall's fragmented API documentation across five product lines into a single reference partners can actually search.

---

## The problem

SonicWall's public APIs are real and well-documented, but they live in five separate places — NSM, SonicOS, Capture Client, MySonicWall, and Cloud Secure Edge each publish their own docs, in their own format, with their own authentication model. Finding one endpoint means knowing which of five sites to check first. Getting credentials means learning that MySonicWall issues a shared key for three of the five products while Cloud Secure Edge runs on an entirely separate system — something nothing currently explains in one place.

## What this prototype covers

- **A single searchable catalog** spanning all five products, built from real endpoints pulled directly from each product's live public documentation — not placeholder data
- **Category and method filtering** so a partner can narrow from thousands of endpoints to the handful they need, by product, by category, or by HTTP verb
- **Per-product authentication guidance** that reflects how credentials actually work today, including the shared MySonicWall key path and Cloud Secure Edge's separate Command Center flow
- **One entry point for getting an API key**, instead of five different starting points depending on which product a partner happens to land on first

## How I approached it

I built this as a working prototype rather than a spec document, because navigation and information architecture problems are hard to evaluate on paper. Putting a real, clickable version in front of the actual data surfaced structural questions — like the fact that "public" and "documented" aren't always the same thing, and that credential models differ enough across products to need their own explanation — that a static mockup wouldn't have exposed.

Every endpoint in this prototype was pulled from each product's currently published documentation, not invented for the demo. The goal was to test whether a partner could find what they needed and understand how to authenticate without opening a support ticket — and to have something concrete for that conversation instead of a description of one.

---

**Role:** Product Manager. I owned the requirements, information architecture, and interaction design, and built this prototype myself.

**Stack:** HTML, CSS, JavaScript
