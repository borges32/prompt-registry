---
nome: Padronizar Comunicação de Alertas
descricao: Converte um snapshot de alertas brutos de monitoramento em comunicados de incidente padronizados com alerta, impacto, hipótese, ação imediata e escalonamento
versao: 1.0.0
tags: [sre, incidentes, alertas, comunicacao, observabilidade]
inputs:
  - nome: snapshot_alertas
    descricao: Snapshot de alertas brutos enviado pelo sistema de monitoramento, a ser convertido para o padrão de 5 campos
---

# Padronizar Comunicação de Alertas

## Objetivo

Transformar um snapshot de alertas brutos do sistema de monitoramento em comunicados de incidente padronizados. Cada alerta sai com cinco campos fixos (ALERTA, IMPACTO, HIPÓTESE INICIAL, AÇÃO IMEDIATA e ESCALAR PARA), em linguagem direta e usando apenas dados presentes no snapshot.

## Quando usar

- Ao receber alertas brutos e precisar comunicar o incidente em formato uniforme.
- Para padronizar a comunicação do plantão entre diferentes serviços e times.
- Para gerar comunicados curtos e objetivos, sem preâmbulo, prontos para colar em um canal de incidentes.

## Exemplo de uso

Os 3 exemplos few-shot do próprio prompt (Relay, Forge, Cerebro) mostram o formato de saída esperado:

```
ALERTA: Relay - taxa de rejeição de ingestão acima de 2% por 5min
IMPACTO: ingestão de telemetry degradada para ~12% dos tenants
HIPÓTESE INICIAL: deploy do Relay às 09:14 reduziu o buffer de ingestão
AÇÃO IMEDIATA: rollback iniciado via Argo CD
ESCALAR PARA: @relay-core se a rejeição não cair em 10min
```

## Limitações conhecidas

_A preencher_
