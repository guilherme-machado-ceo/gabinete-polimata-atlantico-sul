---
title: "Hubstry CaaS"
date: 2026-04-14
tags:
  - compliance
  - rust
  - ECA-Digital
  - ANPD
  - deep-tech
  - SaaS
aliases:
  - CaaS
  - Compliance as a Service
  - Hubstry Compliance Engine
---

# Hubstry CaaS
## Compliance as a Service — ECA Digital

> Engine de conformidade regulatória em Rust para a Lei 15.211/2025,
> com janela de mercado aberta até janeiro de 2027.

---

## O problema

A **Lei 15.211/2025 (ECA Digital)** criou obrigações de conformidade
para plataformas digitais que operam com crianças e adolescentes no Brasil.
A **ANPD** começa o enforcement em **janeiro de 2027**.

A maioria das PMEs e startups brasileiras não tem equipe jurídico-técnica
interna para mapear, auditar e demonstrar conformidade nas 8 categorias
exigidas pela lei. O prazo está correndo.

---

## O que é o Hubstry CaaS

Engine de **compliance automatizado** construído em Rust, com arquitetura
open-core:

- **Core open source** (Apache 2.0) — motor de análise e scoring
- **Regras premium proprietárias** — biblioteca atualizada de regras ECA Digital
- **API e relatórios** — saída estruturada para auditoria e documentação

O engine analisa plataformas digitais contra as 8 categorias de conformidade
da Lei 15.211/2025 e produz um **relatório auditável** com score por categoria,
violações classificadas por severidade e roadmap de adequação.

---

## As 8 categorias de conformidade

1. Verificação de idade
2. Proteção de dados de menores
3. Design ético (dark patterns proibidos)
4. Publicidade direcionada
5. Supervisão parental
6. Moderação de conteúdo
7. Privacidade por design
8. Transparência algorítmica

---

## Arquitetura técnica
Stack: Rust (engine core) · Fly.io (backend) · Vercel (frontend)
Supabase (dados) · Mercado Pago (billing)
Licenciamento: Apache 2.0 (core) + proprietário (regras/API/relatórios)
Modelo: open-core · consultancy-first · SaaS gradual

---

## Modelo de negócio

**Go-to-market: consultoria como porta de entrada.**

Cada engajamento de conformidade (R$ 3.000–8.000) usa o engine como
diferenciador técnico — o cliente paga pela consultoria, recebe o relatório
automatizado como entregável de alto valor percebido.

O SaaS recorrente entra na segunda fase, quando a base de clientes
validados justificar o investimento em self-service.

---

## Parceiros e ecossistema

O Hubstry CaaS opera em parceria técnica com a **Gonçalves et Alii
(Et Alii Tech)** como face comercial e metodológica para o mercado B2B e B2G.

A Hubstry desenvolve e mantém o motor técnico.
A Et Alii Tech empacota o engine em frameworks acessíveis para
o cliente final.

---

## Status atual

- ✅ Arquitetura definida
- ✅ Repositório Rust em desenvolvimento (`hubstry-iso-code`)
- ✅ Parceria Microsoft Founders Hub ativa
- 🔄 Engine core em implementação
- ⏳ MVP para Q3 2026
- 🎯 Janela de mercado: até janeiro de 2027 (enforcement ANPD)

---

*Hubstry Deep Tech — Rio de Janeiro.*
*CNPJ MEI ativo desde 2024.*
