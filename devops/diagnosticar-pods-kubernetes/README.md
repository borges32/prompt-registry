---
nome: Diagnosticar Pods Kubernetes
descricao: Analisa um snapshot de pods, eventos e logs do Kubernetes e entrega a causa raiz provável com ações para o plantão
versao: 1.0.0
tags: [kubernetes, troubleshooting, sre, diagnóstico, incidentes]
inputs:
  - nome: snapshot
    descricao: Snapshot do Kubernetes com status dos pods (STATUS, RESTARTS), eventos e logs, a ser analisado
---

# Diagnosticar Pods Kubernetes

## Objetivo

Analisar um snapshot do Kubernetes (status dos pods, eventos e logs) e identificar a causa raiz provável dos pods em estado problemático. O prompt cruza `STATUS`/`RESTARTS`, eventos e linhas de erro dos logs, e gera um relatório com ações recomendadas para o engenheiro de plantão. Se todos os pods estiverem saudáveis, ele devolve um relatório curto de status saudável.

## Quando usar

- Durante um incidente, para triar rapidamente pods em `CrashLoopBackOff`, `ImagePullBackOff`, `Pending`, `Terminating` ou `OOMKilled`.
- Quando você tem status, eventos e logs de um workload e quer uma causa raiz correlacionada, não apenas o status.
- Para confirmar que uma aplicação está saudável após um deploy ou mudança.

## Exemplo de uso

_A preencher_

## Limitações conhecidas

_A preencher_
