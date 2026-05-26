---
title: "Template — Pipeline"
tags: [template, pipeline, automação, processo, metodologia]
date: 2026-05-26
draft: false
---

# Template — Pipeline

**Pipeline** é uma sequência com estado automatizado — o sistema faz parte do trabalho. Diferente do workflow, o pipeline não precisa de você em cada etapa: ele executa, registra, e alerta quando algo falha.

Use quando o processo tem entrada definida, etapas previsíveis e saída verificável.

> *Regra prática: se você faz o mesmo processo mais de uma vez por semana de forma manual, avalie se ele deveria virar um pipeline.*

---

## Template

```markdown
---
nome: [nome do pipeline]
tipo: pipeline
venture: [qual parte do negócio]
automação: [total / semi-automático / manual-com-script]
stack: [tecnologias envolvidas]
versão: 1.0
última-revisão: [AAAA-MM-DD]
---

## Gatilho
[O que dispara o pipeline?]
- [ ] Push para branch específica
- [ ] Agendamento (cron): [frequência]
- [ ] Webhook: [evento]
- [ ] Input manual: [quem dispara e como]

## Estágios

| # | Nome | Responsável | Input | Output esperado | Falha faz |
|---|------|-------------|-------|-----------------|-----------|
| 1 | [nome] | sistema | [o que entra] | [o que sai] | bloquear |
| 2 | [nome] | sistema | [o que entra] | [o que sai] | alertar |
| 3 | [nome] | sistema | [o que entra] | [o que sai] | rollback |

## Health check
[Como verificar que o pipeline rodou corretamente?
O que você verifica e com qual frequência?]

## Alertas
[Onde vão as notificações de falha? Email, mensagem, dashboard?]

## SLA
[Tempo máximo aceitável para execução completa do pipeline.]

## Rollback
[O que fazer se o pipeline falhar após execução parcial?]

## Notas
[Contexto, histórico, links relacionados]
```

---

## Exemplo preenchido — publicação automática de nota (Obsidian → web)

```markdown
---
nome: publicação Obsidian → Quartz → web
tipo: pipeline
automação: total
stack: Obsidian Git · GitHub Actions · Quartz v4 · GitHub Pages
---

## Gatilho
Push automático do Obsidian Git para o repositório no GitHub.
(Configurado para rodar a cada X minutos ou ao fechar o app)

## Estágios

| # | Nome | Responsável | Input | Output esperado | Falha faz |
|---|------|-------------|-------|-----------------|-----------|
| 1 | commit | Obsidian Git | notas modificadas | commit no repo | alertar via email |
| 2 | build Quartz | GitHub Actions | markdown do vault | HTML estático | bloquear deploy |
| 3 | deploy | GitHub Pages | HTML estático | site atualizado | alertar e manter versão anterior |

## Health check
Acessar URL do site após push e verificar se o conteúdo foi atualizado.
Frequência: spot-check semanal + verificação após publicação relevante.

## Alertas
GitHub Actions envia notificação de falha por email automaticamente.

## SLA
Site atualizado em até 5 minutos após push.
```

---

*← [[workflow|Template Workflow]] · [[ferramenta|Template Ferramenta →]]*
