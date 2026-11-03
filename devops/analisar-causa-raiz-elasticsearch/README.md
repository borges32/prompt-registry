---
nome: Analisar Causa Raiz de Incidente Elasticsearch
descricao: Correlaciona configuração, métricas (2h) e logs de um cluster Elasticsearch via Cerebro e entrega um relatório RCA de incidente que afetou uma aplicação Java
versao: 1.0.0
tags: [sre, elasticsearch, rca, observabilidade, java]
inputs:
  - nome: snapshot_config
    descricao: Dados de configuração do cluster Elasticsearch coletados via Cerebro (heap, GC, thread pools, shards e réplicas)
  - nome: snapshot_metricas
    descricao: Métricas do Cerebro das últimas 2 horas do período do incidente
  - nome: snapshot_logs
    descricao: Trechos de logs de um nó do cluster Elasticsearch / Cerebro do período do incidente
---

# Analisar Causa Raiz de Incidente Elasticsearch

## Objetivo

Determinar a causa raiz de um incidente de degradação ou indisponibilidade de uma aplicação Java integrada a um cluster Elasticsearch. O prompt correlaciona três artefatos do período do problema (configuração do cluster, métricas das últimas 2 horas e logs de um nó, todos via Cerebro) e entrega um relatório RCA estruturado. O relatório separa a causa raiz primária dos sintomas secundários e traz cronologia, matriz de correlação e plano de ação.

## Quando usar

- Após um incidente em que uma aplicação Java degradou ou ficou indisponível e há suspeita do cluster Elasticsearch.
- Quando já se têm a configuração do cluster, as métricas das últimas 2 horas e logs de um nó.
- Para produzir um RCA com estrutura fixa, útil em postmortems.
- Para correlacionar timestamps de logs com oscilações de métricas (Heap, GC, thread pools).

## Exemplo de uso

_A preencher_

## Limitações conhecidas

_A preencher_
