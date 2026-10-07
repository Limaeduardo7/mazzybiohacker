# Source of Truth

Use esta hierarquia para evitar memória divergente.

## 1. Operação viva

Quando disponíveis, estes sistemas vencem snapshots do repositório:
- Notion para registros operacionais, approvals e contexto estruturado
- Drive para documentos técnicos e arquivos compartilhados
- Email / mensageria para a comunicação externa mais recente
- sistemas de CRM / tarefas para status operacional corrente

## 2. GitHub

Este repositório é canônico para:
- regras de operação da IA
- skills
- templates
- identidade e design guide
- documentação de processos
- outputs versionados seguros

## 3. Memória local do workspace

Os arquivos em `_memoria/` devem conter princípios relativamente estáveis, não um dump de todos os negócios ativos.

## Regra de reconciliação

Se um dado operacional mudou fora do GitHub, não sobrescrever a fonte viva com uma versão antiga daqui.

Registrar mudanças duráveis no repositório apenas quando forem regras, aprendizados, padrões ou decisões que devam sobreviver à oportunidade atual.
