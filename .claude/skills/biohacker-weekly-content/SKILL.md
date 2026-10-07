---
name: biohacker-weekly-content
description: Planeja, gera, valida e prepara a semana de conteúdo da Biohacker Foods para Instagram usando o sistema de templates T01–T06.
---

# Biohacker Weekly Content

## Objetivo

Produzir conteúdo internacional consistente, visualmente reconhecível e variado para o Instagram da Biohacker Foods.

## Antes de gerar

Ler:
- `_memoria/empresa.md`
- `_memoria/estrategia.md`
- `_memoria/preferencias.md`
- `identidade/design-guide.md`
- `marketing/README.md`
- `marketing/templates/README.md`
- `marketing/templates/registry.json`

## Mix semanal sugerido

Distribuir temas entre:
- ingredient spotlight
- education / comparison
- application / formulation
- sourcing / origin
- private label / packaging
- brand / commercial CTA

## Template rotation

Cada item deve conter `templateId`.

Ritmo-base recomendado:
`T01 → T02 → T03 → T04 → T01 → T05 → T06`

Regras:
- não repetir o mesmo template em mais de 2 posts consecutivos
- T01 pode aparecer duas vezes na semana porque produto é o núcleo visual
- usar T05 apenas quando houver contexto real de private label / packaging
- usar T06 para fechamento institucional, anúncio ou CTA

## Regras editoriais

- Inglês como padrão.
- Não fazer claims médicos.
- Não inventar ORAC, certificações, origem, estoque ou propriedades funcionais.
- Explicar processo quando relevante.
- CTA B2B.
- Evitar posts genéricos de wellness.

## Formato do planejamento

Arquivo:
`planejamento/semana-AAAA-MM-DD.json`

Cada item:
- `slug`
- `date`
- `category`
- `theme`
- `templateId` — T01 a T06
- `hook`
- `caption`
- `cta`
- `slides`

Exemplo:

```json
{
  "slug": "acai-powder",
  "category": "Ingredient Spotlight",
  "theme": "Açaí Powder",
  "templateId": "T01",
  "hook": "A Brazilian superfruit built for modern formulations.",
  "caption": "...",
  "cta": "Request specifications",
  "slides": []
}
```

Se `templateId` estiver ausente, o renderer tenta inferir a família pelo tema/categoria, mas o planejamento novo deve defini-lo explicitamente.

## Publicação

Quando Buffer estiver configurado:
1. validar
2. renderizar
3. conferir assets
4. agendar
5. registrar IDs retornados
6. arquivar

Nunca afirmar que um post foi agendado sem ID real da plataforma.
