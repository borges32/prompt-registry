---
nome: Diagnosticar Migração de Batch para Tempo Real
descricao: Analisa a documentação de um sistema em processamento em lote (Forge), mapeia gargalos e acoplamentos e compara caminhos arquiteturais para tempo real, com recomendação e bloco de exportação para o próximo passo.
versao: 1.0.0
tags: [arquitetura, batch, streaming, tempo-real, migração]
inputs:
  - nome: dados_do_sistema_e_ambiente
    descricao: Documentação e dados do sistema Forge e de seu ambiente (funcionamento do lote atual, volumetria, janelas de execução, dependências)
---

# Diagnosticar Migração de Batch para Tempo Real

## Objetivo

Dado o snapshot de documentação e ambiente do sistema Forge, o prompt assume o papel de Arquiteto Principal de Sistemas Distribuídos. Ele mapeia o estado atual do processamento em lote (volumetria, janelas, dependências), identifica gargalos e acoplamentos, avalia ao menos dois caminhos arquiteturais para tempo real (ex.: CDC/Debezium, Kafka/RabbitMQ, Flink/Spark, Webhooks/Serverless) e recomenda um deles. Entrega um relatório técnico em Markdown para tech leads, arquitetos e engenheiros do projeto.

## Quando usar

- Ao iniciar a avaliação da migração de um sistema em lote para arquitetura orientada a eventos ou streaming.
- Quando é preciso mapear gargalos e acoplamentos que impedem o tempo real.
- Quando se quer comparar caminhos arquiteturais com prós, contras e uma recomendação justificada.
- Como primeiro passo de uma cadeia de prompts, pois a saída inclui um bloco `<passo1_result>` para alimentar o próximo prompt.

## Exemplo de uso

Substituir `{{dados_do_sistema_e_ambiente}}` pela documentação e pelos dados do ambiente do sistema Forge. A saída é o relatório com mapeamento do estado atual, análise dos caminhos, recomendação técnica e o bloco de exportação.

## Limitações conhecidas

_A preencher_
