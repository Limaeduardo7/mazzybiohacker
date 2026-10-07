---
name: salvar
description: Salva mudanças do workspace no GitHub com commit e push seguro. Use em /salvar, "salvar", "commit", "push" ou "sincronizar".
---

# /salvar

## Workflow

1. Rodar `git status --short`.
2. Se não houver mudanças, informar que está sincronizado.
3. Verificar se nenhum arquivo sensível entrou no diff:
   - .env
   - private/
   - confidential/
   - supplier quotations
   - customer data exports
   - internal pricing
4. Se houver material potencialmente confidencial, parar e pedir revisão.
5. Gerar mensagem de commit curta.
6. `git add` apenas dos arquivos aprovados.
7. `git commit -m "<mensagem>"`.
8. `git push`.

## Guardas

- Nunca usar `git push --force` sem pedido explícito.
- Nunca versionar tokens.
- Nunca usar `git add -A` cegamente quando houver arquivos comerciais locais.
- Se o remoto divergir, oferecer `git pull --rebase` antes de tentar novamente.
