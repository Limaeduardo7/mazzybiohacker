# Biohacker Foods — Instagram Template System

This is the canonical template library for the Biohacker Foods Instagram OS.

All new feed posts and carousels should select one of the six templates below before visual production. The visual references were approved in the October 2026 brand setup; the operational rules in this folder are the source of truth for recreating that look consistently.

## Template registry

| ID | Template | Primary use |
|---|---|---|
| T01 | Ingredient Spotlight | Product / ingredient hero |
| T02 | Educational Comparison | A vs B, process, format, technical education |
| T03 | Application Spotlight | Smoothies, bowls, beverages, formulations, use cases |
| T04 | Origin & Sourcing | Brazil, Amazon, provenance, supply-chain storytelling |
| T05 | Private Label | Packaging, custom formats, brand-ready products |
| T06 | Brand Message | Positioning, announcements, institutional CTA |

## Mandatory visual system

- Canvas: 1080 × 1350 px (4:5)
- Background: Warm Cream `#F7F2E8`
- Primary text: Deep Plum `#3A102C`
- Secondary plum: `#5A123F`
- Accent: Botanical Gold `#B4934E`
- Headline: elegant high-contrast editorial serif
- Supporting copy: clean modern sans-serif
- Photography: premium food/ingredient photography, natural light, shallow depth of field
- Botanical details: restrained gold line-art and real green leaves
- Logo: upper-left by default; never oversized

## Feed rotation

Do not use the same template for more than two consecutive feed posts.

Recommended rhythm:
`T01 → T02 → T03 → T04 → T01 → T05 → T06`

The weekly planner may vary the sequence based on content, but should maintain visual rhythm between product, educational, application, origin, commercial, and institutional posts.

## Selection rules

- Product name / SKU / fruit feature → T01
- X vs Y / freeze-dried vs spray-dried / educational comparison → T02
- Recipe, formulation, smoothie, bowl, beverage, finished-product use → T03
- Brazil, Amazon, farms, origin, traceability, sourcing → T04
- Private label, packaging, formats, branded products → T05
- Company positioning, capabilities, launch, announcement, direct CTA → T06

Each post should declare `templateId` in its planning JSON. If absent, the renderer may infer a template from the content category, but explicit selection is preferred.

## Files

- `registry.json` — machine-readable template metadata
- `T01-ingredient-spotlight.md`
- `T02-educational-comparison.md`
- `T03-application-spotlight.md`
- `T04-origin-sourcing.md`
- `T05-private-label.md`
- `T06-brand-message.md`

Do not create a seventh visual family casually. Extend one of these templates first. A new canonical template requires an explicit brand-system decision.
