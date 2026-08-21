---
title: "NDX CVD — Agregação do Delta de Volume do Índice À Vista"
date: 2026-08-21
draft: false
tags: ["atlas", "NDX CVD", "order flow", "agregação", "microestrutura"]
---

# NDX CVD — Agregação do Delta de Volume do Índice

**Na cosmologia Antigravity:** Combustível da Estrela Central (NDX).
**Em linguagem clássica:** Delta de Volume Cumulativo (CVD) ponderado pelo índice para as 100 empresas do índice NASDAQ-100.

## Como o NDX CVD é Calculado

O índice NASDAQ-100 é uma cesta de ativos e não uma ação única. O indicador **NDX CVD** na telemetria do Heniu é calculado da seguinte forma:

1. **Feed de Negócios:** Leitura contínua das transações de cada um dos 100 componentes do índice.
2. **Classificação de Negócios (Tick Rule / BBO):** Ordens executadas ao preço de Ask (compra agressiva) somam volume (+); ordens executadas ao preço de Bid (venda agressiva) subtraem volume (-).
3. **Ponderação e Agregação:** Os deltas de volume são agregados em tempo real com base nos pesos de cada empresa no índice:
   $$ \text{CVD}_{NDX} = \sum_{i=1}^{100} w_i \cdot (\text{Vol}_{\text{Ask}, i} - \text{Vol}_{\text{Bid}, i}) $$
   onde $w_i$ é o peso da empresa no índice. Dessa forma, megacaps (como Apple e NVIDIA) têm impacto proporcional à sua representatividade no índice.
4. **Reset da Sessão:** A linha de CVD é zerada na abertura da sessão regular às 9:30 ET (15:30 CET / 10:30 BRT), medindo a agressão do fluxo para o pregão atual.

## Unidades e Interpretação Semântica

* **Unidade:** Valores apresentados nos relatórios (ex.: `+162,49M` ou `-175,43M`) representam **NDX Weighted Flow Units (unidades de fluxo ponderado)**. Pela ponderação do índice, não se trata de uma simples contagem bruta de ações disparatadas, mas de um vetor padronizado de pressão agressiva.
* **CVD NÃO é "entrada/saída de capital":** Em toda negociação, dinheiro e ações trocam de mãos simetricamente. O CVD não mede aportes externos, mas sim o **signed aggressive order flow** — revelando qual lado (compradores a mercado agredindo o Ask ou vendedores a mercado agredindo o Bid) está pagando o spread para obter liquidez imediata.
* **Divergências NDX / CVD:**
  - Preço cai enquanto o NDX CVD sobe: absorção passiva de vendas agressivas por ordens limite de compra (acumulação).
  - Preço sobe com NDX CVD negativo: distribuição passiva de ordens de venda sobre compras agressivas a mercado.

---

*Entrada do Atlas. Zero sinais de negociação — estritamente física de mercado.*
