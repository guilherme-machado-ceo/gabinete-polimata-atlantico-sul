---
title: "Template — Ferramenta"
tags: [template, ferramenta, stack, metodologia]
date: 2026-05-26
draft: false
---

# Template — Ferramenta

Cada ferramenta no seu stack deveria ter uma função definida, uma justificativa clara e uma alternativa caso falhe. Ferramenta sem propósito explícito é ruído operacional.

> *Regra prática: se você não consegue explicar em uma frase por que usa essa ferramenta, você provavelmente não deveria estar usando.*

---

## Template

```markdown
---
nome: [nome da ferramenta]
tipo: ferramenta
categoria: [dev / pesquisa / publicação / comunicação / negócios / automação]
custo: [gratuito / freemium / pago — valor mensal]
versão: 1.0
última-revisão: [AAAA-MM-DD]
---

## Função no ecossistema
[Para que serve esta ferramenta? Qual problema específico ela resolve?
Uma frase clara. Se precisar de mais de uma frase, a função não está clara.]

## Módulo OS
[Em qual módulo do OS ela atua? Pode ser mais de um.]
- [ ] Aquisição
- [ ] Conversão
- [ ] Entrega
- [ ] Retenção
- [ ] Controle

## Integrações
[Com quais outras ferramentas do stack ela se conecta?
Como os dados ou outputs fluem entre elas?]

## Configurações críticas
[O que precisa estar configurado para funcionar corretamente?
O que, se estiver errado, quebra o processo que depende dela?]

## Fluxo padrão de uso
1. [como usar no dia a dia — passo a passo mínimo]
2.
3.

## Alternativa se indisponível
[O que usar se esta ferramenta cair ou ficar inacessível?
Mesmo que seja manual: "se X cair, fazer Y manualmente até voltar."]

## Critério de substituição
[Em que condições você deveria trocar esta ferramenta por outra?
Ex: custo aumenta acima de X, funcionalidade Y não está disponível, etc.]

## Notas
[Contexto, histórico, links relacionados]
```

---

## Por que documentar ferramentas

Três razões práticas:

**1. Você troca de ferramenta no futuro.** Sem documentação, você não sabe o que vai perder, o que vai manter e o que vai precisar reconfigurar. Com documentação, a migração tem um checklist.

**2. Outra pessoa vai usar.** Mesmo que você seja solofounder hoje, um colaborador, parceiro ou agente de IA vai precisar entender sua stack. A documentação é a ponte.

**3. Você mesmo vai esquecer.** Configurações críticas feitas há seis meses não estão na sua memória. Estão (ou deveriam estar) no documento.

---

## Sinais de que uma ferramenta deveria ser removida do stack

- Você não consegue lembrar por que a adotou
- Ela tem sobreposição de função com outra ferramenta que você já usa
- O custo não é justificado pelo valor gerado
- Ela cria dependências desnecessárias sem benefício claro

---

*← [[pipeline|Template Pipeline]] · [[../index|Voltar ao índice →]]*
