---
name: carrossel
description: Cria posts e carrosséis exclusivamente para o Instagram da Biohacker Foods, em 1080×1350, usando o sistema canônico T01–T06. Use quando o usuário pedir post, carrossel, conteúdo para Instagram ou /carrossel.
---

# /carrossel — Instagram Biohacker Foods

## Dependências

Antes de criar:
- ler `_memoria/empresa.md`
- ler `_memoria/preferencias.md`
- ler `_memoria/estrategia.md`
- ler `identidade/design-guide.md`
- ler `marketing/templates/README.md`
- ler a especificação do template escolhido em `marketing/templates/`

Outputs:
`marketing/conteudo/<tema>-<YYYY-MM-DD>/`

## Passo 1 — Selecionar template

Escolher explicitamente um `templateId`:

- T01 — Ingredient Spotlight
- T02 — Educational Comparison
- T03 — Application Spotlight
- T04 — Origin & Sourcing
- T05 — Private Label
- T06 — Brand Message

Seleção padrão:
- produto/ingrediente → T01
- comparação/educação técnica → T02
- uso/aplicação/formulação → T03
- origem/sourcing → T04
- embalagem/private label → T05
- institucional/CTA/anúncio → T06

Não criar uma sétima família visual sem decisão explícita do usuário.

## Formatos

### Carrossel
- 1080×1350
- 5 a 8 slides por padrão
- slide 1: capa
- slides internos: um insight por slide
- slide final: CTA discreto

### Post único
- 1080×1350
- uma ideia central
- seguir integralmente a anatomia do template escolhido

## Direção visual

Aplicar:
- Warm Cream #F7F2E8
- Deep Plum #3A102C
- Botanical Gold #B4934E
- serif editorial para títulos
- sans-serif limpa para texto funcional
- fotografia premium de frutas, ingredientes, pós e aplicações
- composição limpa, natural e internacional

Evitar:
- estética fitness
- neon
- excesso de ícones
- templates genéricos de IA
- cápsulas genéricas
- poluição visual

## Texto

Idioma padrão: inglês.

Regras:
- capa com no máximo 8 palavras
- pouco texto por slide
- sem claims médicos
- não inventar certificações, origem, composição ou benefício técnico
- CTA final discreto

## Legenda

Sempre gerar `legenda.md`.

Estrutura:
1. hook
2. contexto curto
3. principal aprendizado/benefício
4. CTA
5. hashtags relevantes, sem excesso

## Workflow

1. Definir tema e ângulo.
2. Selecionar `templateId`.
3. Ler a especificação desse template.
4. Escrever o conteúdo.
5. Mostrar o texto para aprovação quando o pedido for manual.
6. Criar o visual em HTML/CSS ou pelo pipeline semanal.
7. Renderizar PNGs em 1080×1350.
8. Conferir capa, slide intermediário e CTA final.
9. Salvar `templateId` no `conteudo.json`.
10. Se o usuário pedir publicação, seguir `/aprovar-post`.

## Regras

- Instagram somente.
- Não gerar versões para TikTok, LinkedIn, Facebook ou blog.
- Não oferecer automaticamente versão de blog.
- Não mudar a identidade visual sem atualizar o design guide e o template registry.
