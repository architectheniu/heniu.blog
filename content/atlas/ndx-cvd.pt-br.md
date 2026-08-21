---
title: "NDX CVD — Agregação do Volume Delta do Índice à Vista"
date: 2026-08-21
draft: false
tags: ["atlas", "NDX CVD", "order flow", "agregação", "microestrutura"]
---

# NDX CVD — Agregação do Delta de Volume do Índice

**Na Cosmologia Antigravity:** Combustível da Estrela Central (NDX).
**Na Linguagem Clássica:** Delta de Volume Cumulativo (CVD) ponderado e agregado para as 100 ações constituintes do NASDAQ-100.

## Como o NDX CVD é Construído

O índice NASDAQ-100 é uma cesta de ativos. A métrica **NDX CVD** é calculada da seguinte forma:

1. **Feed de Negócios:** Leitura contínua dos negócios executados nas 100 empresas do índice.
2. **Classificação do Agressor:** Ordens no Ask (compradores agressivos) somam volume; ordens no Bid (vendedores agressivos) subtraem volume.
3. **Agregação e Ponderação:** Os deltas são somados em tempo real de acordo com o peso de cada empresa no índice, gerando uma linha unificada de fluxo para o mercado à vista.
4. **Reset da Sessão:** A linha de CVD é zerada na abertura do pregão regular às 9:30 ET.

## Interpretação

Valores reportados (ex: `+162,49M` ou `-175,43M`) quantificam o total líquido de ações transacionadas com agressão na sessão.

* **Divergência NDX / CVD:** Queda no índice com CVD positivo indica absorção passiva de vendas. Alta no índice com CVD negativo indica distribuição passiva na demanda compradora.

---

*Ficha do Atlas. Zero sinais — apenas a física do Sistema.*
