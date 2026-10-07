---
name: comparar-fornecedores
description: Compara fornecedores para uma demanda específica usando custo, spec, documentos, capacidade, logística e risco. Use quando houver duas ou mais opções de supply.
---

# /comparar-fornecedores

## Matriz

Comparar:
- exact product/spec match
- origin
- price basis
- MOQ
- Incoterm
- lead time
- stock / capacity
- packaging
- certificates
- TDS / COA completeness
- sample support
- response quality
- logistics complexity
- commercial risk

## Output

Entregar:
1. ranking
2. melhor opção para o caso
3. melhor alternativa
4. gaps que impedem decisão
5. próximos passos

## Regras

- Normalizar unidade, moeda e Incoterm antes de comparar preço.
- Não declarar uma opção "mais barata" se as bases não forem comparáveis.
- Nunca mostrar custo confidencial em material destinado ao comprador.
