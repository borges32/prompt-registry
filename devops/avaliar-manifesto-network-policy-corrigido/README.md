---
nome: Avaliar Manifesto de NetworkPolicy Corrigido
descricao: Audita um manifesto Kubernetes corrigido por modelo de linguagem, verificando fidelidade aos dados, conformidade com NetworkPolicy, validade do YAML e resolução de divergências, e emite nota de 0.0 a 5.0 com parecer final.
versao: 1.0.0
tags: [kubernetes, network-policy, avaliação, segurança, qualidade]
inputs:
  - nome: snapshot_inputs_originais
    descricao: Entradas originais da correção (manifesto, padrão de NetworkPolicy e lista de serviços e labels permitidos)
  - nome: snapshot_resultado_correcao
    descricao: Resposta gerada pela correção (relatório e manifesto corrigido) a ser avaliada
---

# Avaliar Manifesto de NetworkPolicy Corrigido

## Objetivo

Avaliar criticamente o manifesto Kubernetes corrigido produzido por um modelo de linguagem a partir de um prompt de correção de NetworkPolicy, comparando-o com os dados originais. A avaliação segue quatro critérios ponderados: fidelidade aos dados (40%), conformidade com NetworkPolicy (30%), sintaxe e validade do YAML (15%) e resolução de divergências (15%). O resultado é uma tabela de pontuação, uma nota final de 0.0 a 5.0 e um parecer (aprovado para deploy ou reprovado).

## Quando usar

- Após executar o prompt de correção de manifesto de NetworkPolicy, para validar a resposta antes do deploy.
- Para detectar alucinação de serviços, labels, namespaces ou portas no manifesto gerado.
- Para obter uma nota objetiva e um parecer de aprovação ou reprovação do manifesto.

## Exemplo de uso

_A preencher_

## Limitações conhecidas

_A preencher_
