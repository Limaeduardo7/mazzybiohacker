---
name: aprovar-post
description: Faz a revisão final de um post/carrossel da Biohacker Foods e, após confirmação, envia exclusivamente ao Instagram via Buffer. Use quando o usuário disser "aprovar post", "pode publicar", "posta esse" ou "/aprovar-post".
---

# /aprovar-post — Aprovação final do Instagram

## Workflow

1. Localizar o conteúdo em `marketing/conteudo/`.
2. Validar:
   - PNGs 1080×1350
   - ordem dos slides
   - legenda
   - ortografia
   - identidade visual
   - ausência de claims não sustentados
3. Mostrar ao usuário:
   - tema
   - quantidade de slides
   - legenda
   - data/hora prevista, se houver
4. Pedir confirmação explícita em uso manual.
5. Após aprovação, chamar o fluxo `/agendar-buffer`.
6. Registrar o ID real retornado pelo Buffer.

## Guardas

- Instagram somente.
- Não publicar blog, Facebook, LinkedIn ou TikTok.
- Não publicar se faltar slide, legenda ou validação.
- Não afirmar sucesso sem ID real da plataforma.
- Se o usuário apenas disser "aprovado" sem pedir publicação/agendamento, marcar como aprovado e parar.
