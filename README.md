# Biohacker Foods — Instagram OS

Sistema focado exclusivamente na operação de Instagram da Biohacker Foods.

## O que este repositório faz

- planeja a semana de conteúdo
- gera carrosséis 1080×1350
- aplica a identidade visual da Biohacker
- prepara legendas em inglês
- valida o lote semanal
- renderiza os slides em PNG
- agenda/publica no Instagram via Buffer quando configurado
- registra IDs reais de publicação e arquiva o lote no GitHub

## Estrutura

- `_memoria/` — contexto editorial e posicionamento
- `identidade/` — design guide e assets
- `marketing/` — conteúdo gerado
- `planejamento/` — planos semanais em JSON
- `public/` — mídia pública usada no agendamento
- `scripts/` — renderização, validação e Buffer
- `saidas/` — registros de agendamento
- `.claude/skills/` — skills do fluxo de Instagram

## Skills

- `/biohacker-weekly-content`
- `/carrossel`
- `/agendar-buffer`
- `/aprovar-post`
- `/abrir`
- `/salvar`
- `/atualizar`

## Pipeline semanal

```bash
npm install
npx playwright install chromium

npm run weekly:validate -- --input planejamento/semana-YYYY-MM-DD.json
npm run weekly:render -- --input planejamento/semana-YYYY-MM-DD.json
npm run weekly:schedule -- --input planejamento/semana-YYYY-MM-DD.json
npm run weekly:archive -- --input planejamento/semana-YYYY-MM-DD.json
npm run buffer:discover
```

## Antes de publicar

Adicionar a logo oficial em:

`identidade/assets/logo-biohacker-foods.png`

Configurar localmente o `.env`:

```env
BUFFER_ACCESS_TOKEN=
BUFFER_ORGANIZATION_ID=
BUFFER_INSTAGRAM_CHANNEL_ID=
```

`OPENAI_API_KEY` é opcional e só é necessária se o fluxo local usar geração de imagens por API.

Nunca versionar o `.env`.

## Direção editorial

O Instagram deve posicionar a Biohacker Foods como uma marca premium de superfoods e ingredientes de frutas, com estética sofisticada e apelo internacional.

Idioma padrão: inglês.

Evitar conteúdo genérico de academia, claims médicos e visual de suplemento fitness.
