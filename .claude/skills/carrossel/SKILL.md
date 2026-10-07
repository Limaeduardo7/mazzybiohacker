---
name: carrossel
description: Cria posts e carrosséis exclusivamente para o Instagram da Biohacker Foods, em 1080×1350, seguindo a identidade visual da marca. Use quando o usuário pedir post, carrossel, conteúdo para Instagram ou /carrossel.
---

# /carrossel — Instagram Biohacker Foods

## Dependências

Antes de criar:
- ler `_memoria/empresa.md`
- ler `_memoria/preferencias.md`
- ler `_memoria/estrategia.md`
- ler `identidade/design-guide.md`

Outputs:
`marketing/conteudo/<tema>-<YYYY-MM-DD>/`

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
- pode usar foto, ingrediente, produto ou composição tipográfica

## Direção visual

Aplicar o design guide da Biohacker:
- warm cream
- deep plum
- botanical gold
- serif editorial para títulos
- sans-serif limpa para texto funcional
- fotografia real de frutas, ingredientes, pós e aplicações
- composição premium, limpa e natural

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

Exemplos de CTA:
- Discover our ingredients
- Request specifications
- Ask about wholesale availability
- Talk to Biohacker Foods

## Legenda

Sempre gerar `legenda.md` junto com o post.

Estrutura:
1. hook
2. contexto curto
3. principal aprendizado/benefício
4. CTA
5. hashtags relevantes, sem excesso

## Workflow

1. Definir tema e ângulo.
2. Escrever o conteúdo do carrossel.
3. Mostrar o texto para aprovação quando o pedido for manual.
4. Criar o visual em HTML/CSS ou pelo pipeline semanal.
5. Renderizar PNGs em 1080×1350.
6. Conferir capa, slide intermediário e CTA final.
7. Salvar legenda e arquivos.
8. Se o usuário pedir publicação, seguir `/aprovar-post`.

## Regras

- Instagram somente.
- Não gerar versões para TikTok, LinkedIn, Facebook ou blog.
- Não oferecer automaticamente versão de blog.
- Não mudar a identidade visual sem atualizar o design guide.
