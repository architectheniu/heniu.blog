---
title: "Opções do QQQ e Esfera de Dyson — IV, Put/Call Ratio e Variação Esperada"
date: 2026-08-21
draft: false
tags: ["atlas", "opções", "QQQ", "IV", "Put/Call", "Expected Move", "Esfera de Dyson"]
---

# Opções do QQQ e Esfera de Dyson (Options Surface)

**Na cosmologia Antigravity:** Esfera de Dyson / Escudos Gravitacionais e Campo de Volatilidade.
**Em linguagem clássica:** Parâmetros da superfície de volatilidade implícita (IV), estrutura de volume de opções e intervalo esperado de oscilação (Expected Move) no ETF QQQ.

## O que é a Esfera de Dyson

O fundo de índice Invesco QQQ Trust (QQQ) é o principal veículo de liquidez e hedge para o NASDAQ-100. O mercado de opções do QQQ constitui um imenso amortecedor institucional onde formadores de mercado (dealers) e fundos negociam risco e volatilidade.

## Métricas Principais na Telemetria

### 1. Volatilidade Implícita (Implied Volatility — IV)
* **O que mede:** Volatilidade implícita anualizada de 30 dias (composta / at-the-money) precificada pelo mercado de opções.
* **Significado:** IV mais alta reflete prêmios de opções mais caros e expectativa de oscilações mais amplas; IV baixa indica compressão de volatilidade.

### 2. Put/Call Volume Ratio (Razão de Volume Put/Call)
* **Definição:** A relação entre o volume negociado de opções de venda (Put) e opções de compra (Call) na sessão:
  $$ \text{P/C Ratio} = \frac{\text{Volume Put}}{\text{Volume Call}} $$
* **Rigor Interpretativo:** Um valor de `P/C = 1,32` significa estritamente que foram negociados 1,32 contratos Put para cada contrato Call. **Essa métrica NÃO comprova intenção direcional unilateral:**
  - Pode indicar compra de puts (proteção de carteira ou aposta em queda),
  - Pode indicar venda de puts (coleta de prêmio / posição compradora de dealers),
  - Pode resultar de operações estruturadas com travas ou arbitragem.
  Na ponte do Heniu, o P/C é tratado estritamente como **assimetria bruta de volume contratual**.

### 3. Variação Esperada (Expected Move)
* **Definição:** A faixa estatística de preço precificada pelas opções para determinado horizonte:
  $$ \text{Expected Move} \approx \text{Preço} \times \text{IV} \times \sqrt{\frac{\text{DTE}}{365}} $$
* **Nos Registros:** A faixa apresentada (ex.: `Faixa 703,27 – 718,59`) representa a banda de desvio padrão ($\pm 1\sigma$), cobrindo o intervalo de ~68% de probabilidade precificado pelo mercado.

## O que a Telemetria de Opções NÃO Faz

A superfície de opções não é uma barreira intransponível. Rompimentos além do intervalo esperado ocorrem com frequência diante de eventos macroeconômicos inesperados.

---

*Entrada do Atlas. Zero sinais de negociação — estritamente física de mercado.*
