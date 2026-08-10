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

Uma parte enorme do capital do mercado — fundos de índice, ETFs — liquida por definição ao **preço de fechamento**. Suas ordens entram num leilão especial de fechamento, e alguns minutos antes do fim da sessão a bolsa publica o **desequilíbrio**: quanto há a mais para comprar do que para vender (ou o inverso). É o único momento do dia em que o grande capital **precisa mostrar as cartas** — o fluxo é declarado, não inferido.

Por isso a janela do MOC costuma ser o momento gravitacionalmente mais denso da sessão: dezenas ou centenas de milhões de ações procuram contraparte em poucos minutos. O preço de fechamento resultante vira a referência de todo o dia seguinte.

## Como medimos na ponte de comando

Heniu lê o valor líquido do desequilíbrio na janela MOC e o trata por limiares fixados na configuração do sistema: um excedente em torno de ±50M é um sinal forte de pressão direcional no fechamento, e ±150M é um evento classe singularidade (o "Martelo MOC"). A leitura colore a descrição do vetor do sistema de ~15:50 do horário da bolsa até a noite — porque a pressão do fechamento também descreve a postura com que o capital entra no dia seguinte.

## O que o MOC não faz

Ele não profetiza a sessão de amanhã — mede a pressão de liquidação de hoje. Às vezes um Martelo MOC gigante é absorvido sem deixar rastro; às vezes um desequilíbrio pequeno termina em um grande movimento. Neste blog, o MOC é a descrição da força presente no leilão — nada mais.

---

*Uma carta do Atlas. Zero sinais — apenas a física do Sistema.*
