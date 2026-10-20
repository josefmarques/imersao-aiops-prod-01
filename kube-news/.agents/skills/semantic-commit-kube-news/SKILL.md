---
name: semantic-commit-kube-news
description: >
  Regras de commit específicas deste monorepo (kube-news, boilerplate-k8s-aiops
  e prompt-e-contexto-na-pratica). Complementa a skill global semantic-commit
  com os escopos válidos e as convenções locais. Use ao gerar ou revisar
  mensagens de commit neste repositório.
---

# Semantic Commit — kube-news

Aplique primeiro a skill global `semantic-commit`. Esta skill define apenas os deltas deste repositório.

## Escopos válidos

| Escopo | Diretório |
|---|---|
| `kube-news` | `kube-news/` |
| `boilerplate-k8s-aiops` | `boilerplate-k8s-aiops/` |
| `prompt-e-contexto-na-pratica` | `prompt-e-contexto-na-pratica/` |

- Use o escopo do diretório tocado.
- Mudança transversal a mais de um diretório: omita o escopo ou use o escopo predominante, nunca empilhe escopos.
- Skills em `kube-news/.agents/skills/` pertencem ao escopo `kube-news`.

## Convenções locais

- Mensagens em português.
- Formato observado no histórico: `tipo(escopo): descrição`.
- Sem hashtags, tags promocionais ou sufixos obrigatórios na mensagem.
- Não misture mudanças de diretórios diferentes no mesmo commit quando elas tiverem intenções distintas.
- Nunca execute o commit sem aprovação explícita do usuário.

## Exemplos

```text
feat(kube-news): adiciona busca de notícias por termo
fix(boilerplate-k8s-aiops): corrige coleta de eventos do namespace
docs(prompt-e-contexto-na-pratica): atualiza exemplos de prompts
chore(kube-news): atualiza skills do projeto
```
