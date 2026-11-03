---
nome: Planejar Migração Incremental de Batch para Tempo Real
descricao: Define a estratégia de rollout e o roadmap passo a passo da migração incremental do Forge, com coexistência entre lote e tempo real, matriz de riscos, plano de rollback e bloco de exportação para o próximo passo.
versao: 1.0.0
tags: [migração, rollout, rollback, sre, tempo-real]
inputs:
  - nome: resultado_prompt_1
    descricao: Resultado do diagnóstico do Forge (saída do passo anterior), usado como base para definir a estratégia de transição
---

# Planejar Migração Incremental de Batch para Tempo Real

## Objetivo

Com base no diagnóstico já concluído do sistema Forge, o prompt assume o papel de Especialista em Migração de Sistemas e SRE. Ele compara ao menos duas estratégias de transição (ex.: Strangler Fig / dual-run vs. cutover direto), escolhe uma com foco em redução de risco e suporte a rollback, e entrega um roadmap incremental em quatro fases (preparação, coexistência/dual run, cutover e desativação do lote), mais uma matriz de riscos com plano de fallback por fase.

## Quando usar

- Depois de concluído o diagnóstico de arquitetura do Forge, para definir como migrar sem parada do negócio.
- Quando é preciso garantir coexistência entre processamento em lote e tempo real durante a transição.
- Quando se quer um plano de rollout com riscos e rollback por fase para equipes de desenvolvimento, SRE/DevOps e gestão.
- Como segundo passo de uma cadeia de prompts, pois a saída inclui um bloco `<passo2_result>` para alimentar o próximo prompt.

## Exemplo de uso

Substituir `{{resultado_prompt_1}}` pelo resultado do diagnóstico do Forge. A saída é o plano com análise de estratégias, escolha justificada, roadmap em quatro fases, matriz de riscos com rollback e o bloco de exportação.

## Limitações conhecidas

_A preencher_
