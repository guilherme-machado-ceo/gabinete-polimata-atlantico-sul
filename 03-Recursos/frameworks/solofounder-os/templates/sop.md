---
title: "Template — SOP (Standard Operating Procedure)"
tags: [template, sop, processo, metodologia]
date: 2026-05-26
draft: false
---

# Template — SOP

**SOP** (Standard Operating Procedure) é a documentação de um processo que você quer que aconteça da mesma forma toda vez — seja por você, por uma ferramenta, ou por outra pessoa no futuro.

Você não precisa de um manual corporativo. Precisa de algo honesto sobre o que realmente acontece, simples o suficiente para ser seguido sem pensar, e completo o suficiente para ser entendido por alguém que nunca viu o processo.

> *Regra prática: se você fez o mesmo processo mais de três vezes, merece um SOP.*

---

## Como usar este template

1. Copie o bloco abaixo para um novo arquivo em `/processos/interno/`
2. Preencha cada campo honestamente (o que realmente acontece, não o que deveria)
3. Execute o processo seguindo o SOP pela primeira vez
4. Ajuste o que não bateu com a realidade
5. Só depois use como referência permanente

---

## Template

```markdown
---
nome: [ex: atendimento inicial de lead]
tipo: SOP
módulo-os: [aquisição / conversão / entrega / retenção / controle]
venture: [qual parte do negócio]
frequência: [diário / semanal / sob demanda]
tempo-estimado: [X min]
responsável: [nome]
versão: 1.0
última-revisão: [AAAA-MM-DD]
automação-futura: [o que pode ser automatizado neste SOP?]
---

## Objetivo
[Qual resultado este SOP garante quando seguido corretamente?
Seja específico: não "atender bem o cliente", mas "responder em até 2h
com qualificação inicial e registrar no pipeline".]

## Gatilho
[O que dispara este SOP? Condição ou evento específico.
Ex: "Novo lead entra via WhatsApp ou email".]

## Ferramentas
[Lista das ferramentas envolvidas na execução]

## Passos
1. [ação concreta — sem ambiguidade]
2. [ação concreta]
3. [ação concreta]

## Métrica
[O que você mede para saber se este SOP está funcionando bem?
Ex: tempo de resposta, taxa de conversão para próxima etapa.]

## Definição de pronto
[Como você sabe que terminou com sucesso?
Ex: "Lead registrado no pipeline com origem identificada e resposta enviada."]

## Exceções e fallback
[O que fazer quando algo foge do fluxo normal?
Ex: "Se o lead não responder em 48h, enviar uma segunda mensagem.
Se não responder em 7 dias, arquivar como inativo."]

## Notas
[Contexto, histórico, links relacionados]
```

---

## Exemplo preenchido — atendimento inicial de lead

```markdown
---
nome: atendimento inicial de lead
tipo: SOP
módulo-os: aquisição
frequência: sob demanda
tempo-estimado: 15 min
responsável: [founder]
versão: 1.0
última-revisão: 2026-05-26
automação-futura: resposta inicial pode virar template pré-configurado no WhatsApp Business
---

## Objetivo
Responder todo lead inbound em até 2h com mensagem de qualificação
e registrar origem no pipeline.

## Gatilho
Novo contato via WhatsApp, email ou formulário de contato.

## Ferramentas
WhatsApp Business · planilha ou CRM de pipeline · pasta de leads no vault

## Passos
1. Identificar canal de entrada e salvar contexto (o que disse, de onde veio)
2. Classificar: lead frio (só curiosidade), morno (interesse específico), quente (dor clara)
3. Enviar mensagem de resposta com as 3 perguntas de qualificação
4. Registrar no pipeline com: data, canal, classificação inicial
5. Aguardar resposta — se não vier em 48h, enviar follow-up único

## Métrica
Tempo médio de primeira resposta · % de leads que respondem à qualificação

## Definição de pronto
Lead registrado no pipeline + mensagem de qualificação enviada.

## Exceções
Lead com dor muito clara e urgência alta: agendar call antes de
completar qualificação por escrito.
Lead sem resposta após follow-up: arquivar como inativo após 7 dias.
```

---

*← [[../pipeline|Pipeline]] · [[workflow|Template Workflow →]]*
