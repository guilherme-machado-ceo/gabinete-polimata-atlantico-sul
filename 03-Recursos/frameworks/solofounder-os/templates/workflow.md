---
title: "Template — Workflow"
tags: [template, workflow, processo, metodologia]
date: 2026-05-26
draft: false
---

# Template — Workflow

**Workflow** é uma sequência de ações com decisões humanas — diferente do SOP (que é um procedimento repetível) e do Pipeline (que é automatizado). Um workflow tem bifurcações, julgamentos, contexto.

Use quando o processo precisa de você pensando, não só executando.

> *Regra prática: se o processo tem "depende" no meio, provavelmente é um workflow, não um SOP.*

---

## Template

```markdown
---
nome: [nome do workflow]
tipo: workflow
módulo-os: [aquisição / conversão / entrega / retenção / controle]
venture: [qual parte do negócio]
cadência: [diário / semanal / sob demanda]
versão: 1.0
última-revisão: [AAAA-MM-DD]
---

## Gatilho de início
[Qual condição ou evento ativa este workflow?
Seja específico: não "quando preciso" mas "quando [condição concreta] ocorre".]

## Pré-condições
- [ ] [o que precisa estar pronto antes de começar]
- [ ] [o que precisa estar disponível]

## Etapas

### Etapa 1 — [nome]
[Ação concreta. Se houver decisão, especifique os critérios:]
- Se [condição A] → [caminho A]
- Se [condição B] → [caminho B]

### Etapa 2 — [nome]
[Ação concreta]

### Etapa 3 — [nome]
[Ação concreta]

## Critério de conclusão
[Como você sabe que este workflow terminou com sucesso?]

## Exceções
[O que fazer quando algo foge do fluxo esperado?]

## Automação possível
[Qual etapa poderia virar pipeline automático no futuro?]

## Notas
[Contexto, histórico, links relacionados]
```

---

## Diferença prática entre SOP e Workflow

| | SOP | Workflow |
|---|---|---|
| **Quando usar** | Processo repetível sem variação | Processo com decisões e contexto |
| **Quem executa** | Qualquer um com o documento | Você (ou alguém com julgamento) |
| **Tempo** | Estimável com precisão | Variável |
| **Exemplo** | Responder lead em 2h | Elaborar proposta comercial |
| **Resultado** | Sempre o mesmo | Varia conforme contexto |

---

*← [[sop|Template SOP]] · [[pipeline|Template Pipeline →]]*
