---
name: agendar-buffer
description: Agenda ou publica conteúdo aprovado exclusivamente no Instagram da Biohacker Foods via Buffer. Use quando o usuário pedir para agendar, colocar na fila ou publicar um post/carrossel.
---

# /agendar-buffer — Instagram via Buffer

## Pré-requisitos

- `.env` local com:
  - `BUFFER_ACCESS_TOKEN`
  - `BUFFER_ORGANIZATION_ID`
  - `BUFFER_INSTAGRAM_CHANNEL_ID`
- imagens finais já renderizadas
- legenda aprovada
- canal do Instagram validado pelo Buffer

Nunca imprimir ou versionar tokens.

## Validar conexão

```bash
node scripts/weekly-content.mjs discover
```

Considerar a integração válida somente quando o comando retornar a organização e o canal Instagram reais.

## Workflow

1. Localizar o conteúdo aprovado em `marketing/conteudo/`.
2. Conferir:
   - ordem dos slides
   - legenda
   - data/hora
   - canal Instagram
3. Em uso manual, mostrar resumo e pedir confirmação final.
4. Agendar/publicar usando o pipeline Buffer configurado.
5. Capturar o ID real retornado.
6. Registrar metadados não sensíveis em `saidas/`.
7. Relatar sucesso ou erro real.

## Regras

- Instagram é o único canal.
- Não publicar em Facebook, LinkedIn, TikTok ou blog.
- Não afirmar que foi agendado/publicado sem ID real do Buffer.
- Se a API falhar, preservar os arquivos e reportar o erro.
