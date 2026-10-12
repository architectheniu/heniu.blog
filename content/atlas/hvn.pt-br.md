---
title: "HVN — Nó de Alto Volume, a Barreira do Sistema"
date: 2026-10-12
draft: false
tags: ["atlas", "HVN", "perfil de volume", "microestrutura"]
---

# HVN — High Volume Node

**Na cosmologia Antigravity:** uma Barreira — um nó de volume do ecossistema US100.
**Na linguagem clássica:** High Volume Node (nó de alto volume) — um nível de preço em que o mercado negociou um volume excepcionalmente grande nos últimos dias.

## O que um HVN realmente é

Um gráfico comum mostra *quando* houve negócios. Um perfil de volume mostra *onde*: distribui o volume de vários dias pelos níveis de preço. Na maioria dos níveis o preço apenas passa. Em alguns, o mercado negocia por muito tempo e de bom grado, porque os dois lados aceitaram aquele preço — ali cresce um nó, um High Volume Node.

Na cosmologia do Heniu, um nó é uma barreira: um lugar com muito interesse já negociado dos dois lados. Às vezes o preço para ali, às vezes atravessa sem resistência. O Heniu não presume de antemão o que vai acontecer — registra o que aconteceu.

## O HVN no Heniu: todo o ecossistema US100

O Heniu não procura os nós de um único instrumento. Um HVN é um nível em que todo o ecossistema US100 concentrou volume: os contratos futuros NQ (a Sonda), as ações das empresas do índice NDX (a Estrela) e as cotas do fundo QQQ (a Esfera de Dyson). Fora da sessão à vista só o NQ negocia, então só ele acrescenta volume ao perfil nesse período.

Contratos, ações de empresas e cotas de fundo são unidades diferentes, por isso o Heniu não as soma. Cada mercado tem **voz igual** (decisão do Arquiteto): o volume em um nível é dividido pelo volume daquele mercado em toda a janela, e o perfil do ecossistema é a média dessas três participações. Conta onde cada mercado concentra o seu volume, não qual deles negocia mais unidades.

## Como medimos na ponte de comando

- **Eixo comum:** o nível do índice NDX, de 10 em 10 pontos. O Heniu converte o preço do NQ para esse eixo pela base (NQ − NDX) e o preço do QQQ pela proporção (NDX / QQQ). As duas relações são medidas ao vivo na sessão à vista — a mediana das últimas 600 medições — e guardadas para a noite.
- **Horários:** o NQ conta no horário de negociação da CME; o NDX e o QQQ, na sessão à vista.
- **Volume:** o volume do candle de 15 minutos em curso, lido da tela do TradingView por uma extensão do navegador. O candle cresce durante 15 minutos; o Heniu soma cada aumento do seu volume ao nível em que o preço estava naquele momento, e só ao longo da mais longa sequência não decrescente de leituras, por isso picos momentâneos de leitura (por ex. 1.560 → 16.720 → 1.560) nunca entram no perfil.
- **Janela:** os últimos 5 dias de negociação da CME; o dia de negociação começa às 18:00, horário de Nova York.
- **Nó:** um nível que é o mais forte num raio de 2 níveis para cada lado (±20 pontos) e tem pelo menos metade da participação do nível mais forte de todo o perfil.
- **Rompimento:** o preço (no eixo NDX) precisa ficar pelo menos 5 pontos além do nível. Os rompimentos se alternam (para cima, depois para baixo), no máximo uma vez a cada 10 minutos por nível. O Heniu aceita um salto do preço do NQ de mais de 60 pontos só depois que ele se mantém por 2 minutos — um fusível contra erros de leitura.

## Como os HVN aparecem nos Logs

A ponte registra três tipos de eventos, e o Sábio os anota no T-Log seguinte:

- **novo nó** — por ex. "nó HVN no nível NDX 30660 (NQ ≈ 30887)", com a participação de cada um dos três mercados no volume de 5 dias;
- **barreira conquistada** — um nó rompido para cima;
- **suporte derrubado** — um nó rompido para baixo.

O nível está sempre no eixo NDX; entre parênteses vem o seu equivalente aproximado no NQ, porque a base entre o contrato e o índice muda de um dia para outro. Quando os eventos tocam vários níveis vizinhos, o Sábio os junta numa zona, por ex. "30690 – 30730".

## O que um HVN não faz

Não prevê se o preço vai repicar no nó ou atravessá-lo. Um nó é um registro do passado: um mapa dos lugares onde o ecossistema negociou com mais vontade nos últimos 5 dias. Um rompimento é um fato registrado depois do fato, não um sinal. Neste blog, o HVN descreve o terreno por onde o preço se move — nada mais.

---

*Uma carta do Atlas. Zero sinais — apenas a física do Sistema.*
