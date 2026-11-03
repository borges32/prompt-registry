---
nome: Especificar Execução Tática da Migração para Tempo Real
descricao: Transforma o plano de migração do Forge em especificação executável, com padrões de resiliência e garantia de entrega, contratos de eventos, DLQ e retry, plano de observabilidade e checklist de validação do cutover.
versao: 1.0.0
tags: [implementação, resiliência, observabilidade, eventos, cutover]
inputs:
  - nome: resultado_prompt_2
    descricao: Plano de migração do Forge (saída do passo anterior), usado como base para detalhar a execução técnica
---

# Especificar Execução Tática da Migração para Tempo Real

## Objetivo

Com base no plano passo a passo de migração do Forge, o prompt assume o papel de Engenheiro de Software Senior e SRE Lead. Ele compara ao menos duas abordagens de garantia de entrega e resiliência (ex.: at-least-once com idempotência vs. exactly-once), escolhe uma com foco em integridade de dados e complexidade, e entrega um guia operacional (contratos de eventos/schemas, DLQ e retry exponencial, métricas de observabilidade) e um checklist de validação para autorizar o go-live.

## Quando usar

- Depois de definido o plano de migração do Forge, para transformá-lo em especificações executáveis.
- Quando é preciso decidir padrões de garantia de entrega, tratamento de erros e observabilidade antes do cutover.
- Quando se quer um checklist de critérios de aceite para autorizar a virada para tempo real.

## Exemplo de uso

Substituir `{{resultado_prompt_2}}` pelo plano de migração do Forge. A saída é a especificação com análise de abordagens, escolha justificada, guia de execução operacional e checklist `[ ]` de validação do cutover.

## Limitações conhecidas

_A preencher_
