---
name: mapear-rotinas
description: Identifica rotinas repetitivas da Biohacker e converte em skills documentadas. Use em /mapear-rotinas, "automatizar processo", "criar skill" ou "o que dá para automatizar".
---

# /mapear-rotinas

## Workflow

1. Identificar tarefas repetidas nas áreas:
   - commercial
   - suppliers
   - samples
   - documents
   - pricing
   - marketing
2. Para cada rotina, definir:
   - trigger
   - inputs
   - source-of-truth
   - workflow
   - output
   - approval points
   - failure states
3. Conferir se uma skill existente já cobre o caso.
4. Propor no máximo 5 novas skills por rodada.
5. Após aprovação, criar `.claude/skills/<nome>/SKILL.md`.

## Critério

Uma skill deve reduzir variabilidade e erro, não apenas armazenar um prompt grande.
