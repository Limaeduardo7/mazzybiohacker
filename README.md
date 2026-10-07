# Biohacker Foods OS

> Operating system for Biohacker Foods inside Claude Code / Codex.

This repository is the working operating layer for Biohacker Foods: company context, brand identity, commercial workflows, supplier workflows, product knowledge, document standards, pricing governance, marketing systems and reusable AI skills.

## Core idea

The AI should not act as a generic assistant. It should work from Biohacker Foods' operating context, respect commercial rules, preserve source-of-truth boundaries and produce outputs that can be reviewed, versioned and improved.

The system follows a closed-loop model:

**context → decision → execution → capture → review → update**

## Main folders

- `_memoria/` — canonical operating context for the AI workspace
- `identidade/` — brand and visual system
- `commercial/` — lead, account, RFQ, sample and follow-up workflows
- `suppliers/` — supplier qualification and sourcing workflows
- `products/` — product taxonomy and specification model
- `documents/` — technical and compliance document standards
- `pricing/` — commercial pricing governance
- `marketing/` — content and acquisition system
- `skills/` — reusable AI workflows
- `scripts/` — automation and integration helpers
- `saidas/` — generated deliverables
- `dados/` — local input data for analysis

## Important source-of-truth rule

This GitHub repository is the AI execution workspace.

Operational records that change frequently — live leads, supplier records, active opportunities, approvals, tasks and current commercial status — should remain in the systems designated as canonical by Biohacker Foods. The AI must not treat stale repository snapshots as more authoritative than the current operational source.

## Public-repository warning

This repository is currently public.

Do **not** commit:
- API keys or tokens
- customer personal data
- confidential supplier quotations
- internal margin tables
- private pricing matrices
- contracts or restricted certificates
- private commercial correspondence

Use environment variables and private operational systems for sensitive data.

## Start a session

Before any meaningful task, the AI should read:

1. `CLAUDE.md`
2. `_memoria/empresa.md`
3. `_memoria/estrategia.md`
4. `_memoria/preferencias.md`
5. the relevant domain README or skill

Then execute the task and capture durable improvements back into the appropriate workspace file.

## Initial skills

- `biohacker-weekly-content`
- `qualificar-lead`
- `rfq-fornecedor`
- `comparar-fornecedores`
- `responder-lead`
- `pricing`
- `sample-workflow`

The repository is intentionally modular: new routines should become skills when they are repeated often enough to deserve a documented workflow.
