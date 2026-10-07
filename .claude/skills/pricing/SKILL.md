---
name: pricing
description: Estrutura customer pricing para Biohacker Foods a partir de custo e regras comerciais privadas aprovadas. Use quando o usuário pedir preço de venda, margem, tiers, landed estimate ou proposta.
---

# /pricing

## Pré-condição

Obter os dados atuais da fonte privada aprovada:
- supplier cost
- Commercial Pricing Matrix / regra de margem
- logistics estimate
- currency basis
- Incoterm
- relevant fees

## Workflow

1. Normalizar custo por kg/unidade.
2. Separar custo de produto de logística e encargos.
3. Aplicar regra comercial aprovada.
4. Criar tiers coerentes com MOQ e volumes.
5. Calcular margem e sanity-check.
6. Gerar versão interna e versão customer-facing.

## Guardas

- Supplier cost nunca aparece na versão cliente.
- Não versionar pricing confidencial neste repositório público.
- Se a matriz não estiver acessível, não inventar markup; sinalizar o bloqueio.
