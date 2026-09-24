# TAAS Services — Transformation as a Service

An EdTech platform that teaches small and medium businesses how to run a digital transformation, rather than doing it for them.

**Live application:** https://sufian1990.github.io/taas-services/

## The problem

Small business owners know they should adopt cloud tools, data practices and AI, but not what to adopt first, in what order, or whether their team can operate it. They buy tools that go unused, or postpone the decision indefinitely. Limited budget, scarce technical expertise and organizational inertia are the recurring barriers — capability problems rather than software problems.

Consulting transfers the outcome but takes the knowledge away, at thousands per engagement. Course catalogs are affordable but require the learner to diagnose their own gap first, which is exactly what these owners cannot do.

## What this application does

1. **Business profile** — size, sector, and what matters most right now
2. **Assessment** — 20 questions across five dimensions of digital maturity
3. **Report** — each dimension scored out of 100 and banded, weakest identified and interpreted
4. **Learning path** — an ordered module sequence generated from the scores, with the reasoning shown

## The five dimensions

| Dimension | What it measures |
|---|---|
| Digital foundations | Shared storage, backup, individual logins, access removal |
| Operations and workflow | Whether recurring work is tracked in a shared system |
| Data and measurement | What is recorded, and whether anyone reviews it |
| Customer engagement | Contact records, history, follow-up discipline |
| AI readiness | Real use, identified use cases, staff confidence, boundaries |

## How PathFinder decides

The ranking is rules-based, not AI-generated:

- Dimensions are ordered by score, lowest first
- A foundations score below 40 is promoted to first position, because capabilities built on absent foundations do not hold
- The owner's stated priority moves up one position, but never above a foundational gap
- Dimensions scoring 70 or above are excluded

This keeps the recommendation explainable and reproducible. The reasoning shown to the user is the rule that actually fired, not a generated justification.

## Technical notes

Single-file application. Plain HTML, CSS and JavaScript — no framework, no backend, no build step. Answers persist in the browser via `localStorage`, so no data leaves the user's device. Hosted on GitHub Pages.

To run locally, download `index.html` and open it in any browser.

## Scope of this version

This is the MVP. Assessment, scoring and path generation are complete and functional. Three pilot learning modules are authored by November 15; until then the path shows module titles with target durations. CoachBot, the AI agent giving written feedback on module exercises, is specified in the project plan and scheduled for the next build.

## Team

| Member | ID | Role |
|---|---|---|
| Mohammad Abu Sufian | P26385 | Project Manager |
| Mohammad Abdul Karim | P26414 | Technical Lead |
| Umme Habiba | P26403 | Product & AI / Data Manager |
| Nasrin Akter | P26411 | Marketing & Customer Validation |

## Course

STEM505: Project Management with SaaS · Prof. Sungho Kim · Pacific States University · Fall 2026
