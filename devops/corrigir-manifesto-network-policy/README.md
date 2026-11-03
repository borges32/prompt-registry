---
nome: Corrigir Manifesto de NetworkPolicy
descricao: Compara um manifesto Kubernetes com o padrão oficial de NetworkPolicy e a lista de serviços e labels permitidos, e entrega o manifesto corrigido com relatório de divergências e justificativas.
versao: 1.0.0
tags: [kubernetes, network-policy, seguranca, conformidade, iac]
inputs:
  - nome: snapshot_manifesto
    descricao: Manifesto Kubernetes (YAML) a ser revisado e corrigido
  - nome: snapshot_network_policy
    descricao: Padrão oficial de NetworkPolicy (YAML) que o manifesto deve seguir
  - nome: snapshot_servicos
    descricao: Lista oficial de nomes de serviços e labels permitidos no cluster
---

# Corrigir Manifesto de NetworkPolicy

## Objetivo

Revisar um manifesto Kubernetes comparando-o com o padrão oficial de NetworkPolicy e com a lista oficial de serviços e labels do cluster. O resultado é o manifesto corrigido, pronto para `kubectl apply`, acompanhado de um relatório de conformidade. O prompt proíbe inventar serviços, namespaces, portas ou labels que não estejam nos artefatos de entrada.

## Quando usar

- Ao revisar manifestos de NetworkPolicy antes de aplicá-los no cluster.
- Ao alinhar manifestos existentes ao padrão oficial de NetworkPolicy da organização.
- Ao validar se seletores (`podSelector`, `namespaceSelector`) e labels usam apenas serviços permitidos.

## Exemplo de uso

_A preencher_

## Limitações conhecidas

_A preencher_
