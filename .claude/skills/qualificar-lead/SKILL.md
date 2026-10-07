---
name: qualificar-lead
description: Qualifica uma empresa ou contato B2B para a Biohacker Foods e define o próximo passo comercial. Use quando chegar um novo lead, inbound, contato de feira, importador, distribuidor, fabricante ou marca.
---

# /qualificar-lead

## Inputs mínimos

- empresa ou website
- contato, se disponível
- mensagem ou contexto de origem

## Workflow

1. Identificar a empresa e o papel provável na cadeia.
2. Classificar o fit:
   - ingredient house / importer / distributor
   - manufacturer / co-packer
   - foodservice / retail
   - brand / private label
   - trader / broker
   - low-fit / unclear
3. Extrair demanda conhecida:
   - produto
   - formato
   - volume
   - destino
   - certificações
   - timing
4. Marcar gaps.
5. Definir status:
   - QUALIFIED
   - NEEDS_DISCOVERY
   - LOW_FIT
   - DISQUALIFIED
6. Sugerir próximo passo e mensagem curta.

## Regras

- Não inventar volume ou intenção.
- Website/company name é preferível antes de sourcing profundo.
- Se o lead for multi-SKU e recorrente, elevar prioridade.
- Se houver necessidade técnica específica, acionar supplier match em seguida.
