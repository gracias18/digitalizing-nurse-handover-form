# Digitalizing the Nursing Handover Form (IPASS)

## Overview
A redesign of the paper-based nursing shift handover process using a 
digital IPASS form prototype, built to reduce documentation redundancy, 
improve clinical communication, and integrate with existing EHR systems.

## The Problem
Nurses currently maintain two parallel documentation systems: a 
paper-based KARDEX handover form alongside the EHR. This creates:
- **Redundancy** — the same information entered in multiple places
- **Inconsistency** — no standardized format across nurses or shifts
- **Lack of integration** — paper form is disconnected from Epic
- **Cost** — estimated $51,465/year in nurse time and printing costs

## What We Built
A Figma prototype of a digital IPASS nursing handover form designed 
to replace the paper KARDEX and integrate with Epic EHR.

The IPASS framework structures handover around:
- **I** — Illness Severity (acuity level: Stable / Unstable / Critical / 
  Deteriorating)
- **P** — Patient Summary (chief complaint, physical exam by system)
- **A** — Action List (pending tasks and follow-ups)
- **S** — Situation Awareness (contingency planning)
- **S** — Synthesis by Receiver (confirmation of understanding)

## Design Principles Applied (Shneiderman's 8 Golden Rules)
1. **Strive for Consistency** — digital form mirrors paper field 
   structure to ease transition
2. **Enable Shortcuts** — vitals, medications, and allergies 
   auto-populated from Epic
3. **Offer Informative Feedback** — required fields highlighted with 
   "Selection Required!" prompts
4. **Design for Closure** — "Handover report saved successfully!" 
   confirmation; auto-removes from worklist on completion
5. **Simple Error Handling** — descriptive error messages 
   (e.g., "Form cannot be completed without Disposition plan")
6. **Permit Easy Reversal** — edits logged with timestamp and user ID 
   for audit trail accountability
7. **Support Internal Locus of Control** — "Save & Continue Later" 
   draft function; user controls pace
8. **Reduce Memory Load** — visual patient avatar for tubes, lines & 
   drains; auto-populated system fields; no manual transcription

## Technical Architecture
Built on an MVC (Model-View-Controller) architecture:
- **Model** — structured patient data stored in Epic
- **View** — digital form UI/UX (the Figma prototype)
- **Controller** — validates login, fetches and auto-populates data 
  from Epic, documents timestamps, interprets user actions

## Business Case
| | 1 Year | 3 Years |
|---|---|---|
| Cost of current process | $51,465 | $154,395 |
| Cost of future process | $16,458 | $49,374 |
| Transition cost (one-time) | $10,945 | $10,945 |
| **Net savings** | **$24,062** | **$94,076** |

Digitization reduces handover time from 30 minutes to 10 minutes 
per form by eliminating manual transcription. Transition costs include 
Epic customization build (200 hrs) and nurse training (42 nurses).

## Tools
- Figma (prototype)
- Epic EHR (integration concept)

## Team
Group 10: Ziwei, Sapnna, Miriam, Ohene, Grace
MHI2001 — University of Toronto (2025)

## Links
- [View Figma Prototype](https://www.figma.com/make/VkbTP6b3QXEzBrNcuPgSi9/Healthcare-Handover-Form?node-id=0-1&t=A74g2kr7JsrpuKcA-1)
- [View Presentation](MHI2001 - Digitalizing a Form.pdf)
