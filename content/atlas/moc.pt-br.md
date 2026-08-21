---
title: "MOC — o desequilíbrio do fechamento, a Anomalia MOC"
date: 2026-08-10
draft: false
tags: ["atlas", "MOC", "order flow", "microestrutura"]
---

# MOC — Market-On-Close Imbalance

**Na cosmologia Antigravity:** a Anomalia MOC / o Martelo MOC — um golpe gravitacional nos minutos finais do ciclo.
**Na linguagem clássica:** o desequilíbrio de ordens no fechamento — o excedente de demanda ou oferta que a bolsa precisa parear até as 16:00, horário de Nova York.

## O que o MOC realmente é

Uma parte enorme do capital do mercado — fundos de índice, ETFs — liquida por definição ao **preço de fechamento**. Suas ordens entram num leilão especial de fechamento, e a partir das 15:50 ET a bolsa publica o **Net Order Imbalance Indicator (NOII)**: quanto volume permanece não pareado entre compradores e vendedores. É uma das janelas públicas mais limpas para o interesse explicitamente declarado no leilão de fechamento (o Nasdaq Closing Cross) — o fluxo no livro do leilão é registrado, não adivinhado.

Por isso a janela do MOC costuma ser o momento gravitacionalmente mais denso da sessão: dezenas ou centenas de milhões de ações procuram contraparte em poucos minutos. O preço de fechamento resultante vira a referência de todo o dia seguinte.

## Como medimos na ponte de comando

Heniu lê o valor líquido do desequilíbrio na janela MOC e o trata por limiares fixados na configuração do sistema: um excedente em torno de ±50M é um sinal forte de pressão direcional no fechamento, e ±150M é um evento classe singularidade (o "Martelo MOC"). A leitura informa a descrição do vetor do sistema de ~15:50 do horário da bolsa até a noite — documentando o balanço de ordens no fechamento (closing order interest).

## O que o MOC não faz

Ele não profetiza a sessão de amanhã — mede a pressão de liquidação de hoje. Às vezes um Martelo MOC gigante é absorvido sem deixar rastro; às vezes um desequilíbrio pequeno termina em um grande movimento. Neste blog, o MOC é a descrição da força presente no leilão — nada mais.

---

*Uma carta do Atlas. Zero sinais — apenas a física do Sistema.*
