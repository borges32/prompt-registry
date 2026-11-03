---
nome: Decidir Solução para Backpressure
descricao: Analisa um cenário de backpressure em sistemas distribuídos e compara caminhos de solução, entregando um relatório de trade-offs com recomendação e plano de implementação.
versao: 1.0.0
tags: [backpressure, resiliência, sre, mensageria, trade-offs]
inputs:
  - nome: snapshot_cenario
    descricao: Dados do cenário do problema (arquitetura atual, métricas, gargalo e comportamento de produtores e consumidores)
  - nome: snapshot_caminhos
    descricao: Lista dos caminhos possíveis (soluções viáveis propostas) para tratar o problema
---

# Decidir Solução para Backpressure

## Objetivo

Dado um snapshot do cenário do problema (arquitetura, métricas, gargalo, comportamento de produtores e consumidores) e um snapshot com os caminhos de solução viáveis, o prompt assume o papel de Arquiteto de Sistemas Distribuídos e SRE Sênior. Ele diagnostica o gargalo, avalia cada caminho (mecanismo, prós, contras, complexidade, riscos), compara os trade-offs e recomenda uma solução, ou uma combinação híbrida priorizada, em um relatório Markdown estruturado.

## Quando usar

- Quando há backpressure em filas, mensageria ou pipelines de dados e existem várias soluções candidatas (rate limiting, buffering, load shedding etc.).
- Quando é preciso justificar uma decisão técnica com comparação explícita de custo, esforço, impacto na latência e manutenção.
- Quando se quer um plano de implementação com critério de validação ao final da análise.

## Exemplo de uso

Substituir `{{snapshot_cenario}}` pela descrição da arquitetura, métricas e comportamento de produtores e consumidores, e `{{snapshot_caminhos}}` pela lista de soluções viáveis. A saída é o relatório com as seções: análise do cenário, avaliação dos caminhos, matriz de trade-offs, recomendação e plano de implementação.

## Limitações conhecidas

_A preencher_
