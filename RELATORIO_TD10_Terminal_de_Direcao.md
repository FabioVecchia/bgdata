# RELATÓRIO TÉCNICO COMPLETO — SETOR / LINHA **TD10 — TERMINAL DE DIREÇÃO**

**Base documental:** 22 arquivos do repositório `bgdata` (planilhas GBO/Yamazumi, MFV, cronoanálises, fluxogramas, trabalho padrão, projeto de capabilidade, material de TRF e de sincronização de produção).
**Data de consolidação:** 07/10/2025
**Escopo:** diagnóstico do estado atual, capacidade, balanceamento, gargalos, perdas, fluxo de valor, projetos em andamento, investimentos e recomendações.

---

## ÍNDICE

1. [Sumário executivo](#1-sumário-executivo)
2. [O que é o TD10 — contexto e posicionamento](#2-o-que-é-o-td10--contexto-e-posicionamento)
3. [Inventário e mapa dos documentos analisados](#3-inventário-e-mapa-dos-documentos-analisados)
4. [O processo produtivo do TD10 — fluxo detalhado](#4-o-processo-produtivo-do-td10--fluxo-detalhado)
5. [Demanda, takt time e dimensionamento de mão de obra (GBO TERMINAL)](#5-demanda-takt-time-e-dimensionamento-de-mão-de-obra-gbo-terminal)
6. [Capacidade por operação e simulação horária (GBO TD10 Rev06/Rev07)](#6-capacidade-por-operação-e-simulação-horária-gbo-td10-rev06rev07)
7. [Balanceamento de operadores — cenários de GBO](#7-balanceamento-de-operadores--cenários-de-gbo)
8. [Perdas de disponibilidade — o achado mais crítico](#8-perdas-de-disponibilidade--o-achado-mais-crítico)
9. [Montagem / embalagem — cronoanálise e Yamazumi](#9-montagem--embalagem--cronoanálise-e-yamazumi)
10. [Célula Pressmatik — estudo de cenários](#10-célula-pressmatik--estudo-de-cenários)
11. [Laminadoras — operação a jusante](#11-laminadoras--operação-a-jusante)
12. [Mapa de Fluxo de Valor (MFV 335074) e análise Shingo](#12-mapa-de-fluxo-de-valor-mfv-335074-e-análise-shingo)
13. [Trabalho padrão (TPO040 a TPO043)](#13-trabalho-padrão-tpo040-a-tpo043)
14. [Projeto de capabilidade / MeasurLink (Projeto F4)](#14-projeto-de-capabilidade--measurlink-projeto-f4)
15. [Projeto "Fluxo por Família" — piloto da célula Terminal](#15-projeto-fluxo-por-família--piloto-da-célula-terminal)
16. [Setup / Troca Rápida de Ferramentas (TRF)](#16-setup--troca-rápida-de-ferramentas-trf)
17. [Ergonomia e antropometria dos postos](#17-ergonomia-e-antropometria-dos-postos)
18. [Referencial de PPCP (workshop de sincronização)](#18-referencial-de-ppcp-workshop-de-sincronização)
19. [Diagnóstico consolidado — as 10 perdas estruturais do TD10](#19-diagnóstico-consolidado--as-10-perdas-estruturais-do-td10)
20. [Plano de ação recomendado](#20-plano-de-ação-recomendado)
21. [Lacunas, inconsistências e cuidados com os dados](#21-lacunas-inconsistências-e-cuidados-com-os-dados)
22. [Glossário](#22-glossário)
23. [Anexo A — Tabelas-fonte integrais](#anexo-a--tabelas-fonte-integrais)

---

## 1. SUMÁRIO EXECUTIVO

O **TD10** é a primeira linha (célula) de fabricação da família **Terminal de Direção**, operando **usinagem de pino + usinagem de caixa/cachimbo + Equiptop (furo e rosca)**, seguida de **laminação**, **montagem** e **embalagem**. É a linha escolhida como **piloto** de três iniciativas estratégicas simultâneas: *Fluxo por Família*, *Projeto F4 / MeasurLink (capabilidade online)* e *Rumo ao Defeito Zero*.

### Os números-chave

| Indicador | Valor | Fonte |
|---|---|---|
| Demanda mensal | **62.332 peças/mês** | GBO TERMINAL |
| Dias úteis considerados | 27 | GBO TERMINAL |
| Demanda por turno | **769,5 peças/turno** | GBO TERMINAL |
| Tempo efetivo de operação diária | 28.800 s (8 h) | GBO TERMINAL |
| **Takt time** | **37,43 s/peça** | GBO TERMINAL |
| Tempo de trabalho manual total | **59,76 s/peça** | GBO TERMINAL |
| Nº teórico de operadores | **1,60 → 2** | GBO TERMINAL |
| Eficiência medida (mar/abr) | **69,2 %** | GBO TERMINAL |
| Gargalo da linha | **Pino — 30,3 s (≈119 pç/h)** | GBO Rev07 |
| Takt usado no balanceamento de célula | 28 s (cenários) / 30 s (estado atual) | GBO Rev06/07 |
| Lead time do fluxo de valor (MFV 335074) | **334,1 h ≈ 13,9 dias** | MFV |
| % de valor agregado no MFV | **2,13 %** (0,086 % sem beneficiamento) | MFV |
| Lead time (análise Shingo, Terminal) | **20.347 min = 339 h = 14,1 dias** | SHINGO - AV NAV |
| % processando (Shingo) | **0,007 %** (1,43 min em 14 dias) | SHINGO - AV NAV |
| Distância percorrida pelo material | **870 m** | MFV |
| Perdas de disponibilidade por turno | **28.178 s** contra 26.400 s disponíveis → **106,7 %** | GBO Rev06/07 |
| Investimento MeasurLink TD10 | **R$ 56.419,16** | Projeto de Capabilidade |
| Investimento piloto Fluxo por Família (OCs aprovadas) | **R$ 20.810,27** | Projeto fluxo por família |

### As cinco conclusões centrais

1. **O trabalho manual (59,76 s) é 60 % maior que o takt (37,43 s)** — a linha só fecha a conta com ~2 operadores, e mesmo assim com folga mínima. A composição desse tempo é: **21,2 % agrega valor / 46,7 % necessário mas não agrega valor / 32,1 % desperdício puro**. Ou seja, **~79 % do esforço humano do TD10 não agrega valor ao cliente**.
2. **A soma das paradas planejadas (inspeções, viradas, setups, diário de bordo, quadro) consome 106,7 % do tempo disponível de um turno.** Matematicamente a linha não cabe no turno — é a explicação estrutural da eficiência de 69,2 %.
3. **O gargalo é a usinagem do PINO (30,3 s → 119 pç/h)**, que é justamente a operação com maior tempo de setup acumulado e onde roda o "estudo de viradas". Toda melhoria fora do pino tem retorno marginal.
4. **O fluxo de valor é catastroficamente desbalanceado em tempo**: 14 dias de lead time para ~1,4 min de processamento efetivo. **98 % do lead time é espera por processamento**, não processamento. É um problema de PPCP/lote/sincronização, não de velocidade de máquina.
5. **Há três projetos corretos em curso** (fluxo por família com trilhos roletados e lotes de 450 pç; MeasurLink para eliminar medição manual no gargalo; GBO/Yamazumi para reduzir de 5 para 4 postos na montagem). Eles atacam, respectivamente, o lead time, a disponibilidade do gargalo e o custo de mão de obra. **O que falta é sequenciá-los e medir o resultado combinado.**

---

## 2. O QUE É O TD10 — CONTEXTO E POSICIONAMENTO

### 2.1 Produto

O TD10 fabrica **Terminais de Direção** (também chamado "setor Terminal de Direção"). Os códigos de produto identificados nos documentos:

| Código | Descrição | Onde aparece |
|---|---|---|
| **335074** | Terminal Direção Celta | MFV - Terminal de Direção 335074 - Rev. 00 |
| **335272** | Produto montado (MTD) | Ferramenta GBO + YAMAZUMI |
| **C607176** | Pino (componente forjado/matéria-prima) | MFV |
| **C606099** | Cachimbo (componente forjado) | MFV |

Componentes de montagem citados: **bucha, graxa, tampa, guarda-pó, limitador, porca, anel/abraçadeira, coifa, termo de garantia, saco plástico, cartucho, caixa master, etiquetas**.

Fornecedores de forjado citados: **Eletroforja** (cachimbo — entrega semanal, lead time 20 dias), **TKS**, **Metal Brill** (beneficiamento: desengraxe, jateamento, fosfato e sabão).

### 2.2 Posição na fábrica

O TD10 é **uma das linhas da família "Terminal"**, que no mapa do Projeto F4 contém **TD10, TD20, TD30 e TD40**. A fábrica tem ainda as famílias **Pivô (PA10–PA40, PC10–PC40)**, **Axial (JS10, JS20)**, **Conformação** e **Tirante/Freio (TE10/1, TE10/2)**.

Premissa documentada: *"As máquinas da linha 20 serão agora máquinas da linha 10"* — ou seja, o TD10 absorve recursos do TD20 na reconfiguração por fluxo de família.

### 2.3 Por que o TD10 é o piloto

Da planilha *Projeto fluxo por familia (piloto celula terminal)*, aba **Premissas**:

> *"1 – Escolheu-se as linhas 10 e 40 para lote piloto em função das mesmas não necessitarem movimentação nas máquinas de caixas e as Equiptops somente seriam viradas."*

Ou seja: **menor custo e menor tempo de parada para converter o layout**. Além disso, o TD10 é o gargalo da família e por isso o alvo prioritário do projeto de capabilidade.

---

## 3. INVENTÁRIO E MAPA DOS DOCUMENTOS ANALISADOS

| # | Arquivo | Tipo | Conteúdo essencial | Relevância p/ TD10 |
|---|---|---|---|---|
| 1 | `GBO TERMINAL.xlsx` | XLSX | GBO oficial do TD10: 34 eventos cronometrados, classificação AV/NNAV/D, takt, nº de operadores | ⭐⭐⭐ Direta |
| 2 | `Cópia de Cópia de GBO - TD10 - Rev07.xlsx` | XLSX | Capacidades por operação, simulação horária de WIP (30 h), 13 cenários de balanceamento, perdas de disponibilidade | ⭐⭐⭐ Direta |
| 3 | `!!Cópia de Cópia de GBO - TD10 - Rev07.xlsx` | XLSX | **Duplicata byte-idêntica do item 2** (mesmo MD5) | Redundante |
| 4 | `GBO - TD10 - Rev06-1 - ESTUDO DE VIRADAS - DIA A DIA.xlsx` | XLSX | Revisão anterior do mesmo modelo, com abas "NOVO LAYOUT" | ⭐⭐⭐ Direta |
| 5 | `MFV - Terminal de Direção 335074 - Rev. 00.xls` | XLS | Mapa de Fluxo de Valor completo do produto 335074 | ⭐⭐⭐ Direta |
| 6 | `SHINGO - AV NAV.xlsx` | XLSX | Análise Shingo (AV/NAV) do Terminal — lead time 20.347 min | ⭐⭐⭐ Direta |
| 7 | `Fluxograma Linha 10.pptx` | PPTX | Fluxograma PCP→Logística→Produção da Linha 10 | ⭐⭐⭐ Direta |
| 8 | `Fluxograma do Teste Piloto.pptx` | PPTX | Fluxograma do piloto com regras de sucata/pulmão/trilho | ⭐⭐⭐ Direta |
| 9 | `01 - PROJETO DE CAPABILIDADE TD10 (MeasurLink).pptx` | PPTX | One-page report, investimento, ganhos, fases, Projeto F4 | ⭐⭐⭐ Direta |
| 10 | `Ferramenta GBO + YAMAZUMI - Rev1 (Manipulação 4 operadores).xlsm` | XLSM | Cronoanálise da Montagem MTD 335272, 46 atividades, estado atual x proposta | ⭐⭐⭐ Direta |
| 11 | `GBO Montagem.xlsx` | XLSX | Tempos médios de 11 operações de montagem/embalagem (10 postos) | ⭐⭐⭐ Direta |
| 12 | `Pressmatik/Tempos Pressmatik.xlsx` | XLSX | 4 cenários cronometrados da operação Pressmatik + comparação com takt | ⭐⭐⭐ Direta |
| 13 | `GBO - Laminadoras.xlsx` | XLSX | Dimensionamento das laminadoras (rosca, esfera, macho) | ⭐⭐ Processo a jusante |
| 14 | `Projeto fluxo por familia (piloto celula terminal).xlsx` | XLSX | Premissas, orçamento, cronograma de 72 dias, SCs/OCs | ⭐⭐⭐ Direta |
| 15 | `lista de materiais.xlsx` | XLSX | Materiais e preços dos trilhos roletados / flow racks | ⭐⭐ Suporte |
| 16 | `fluxo macro.xlsx` | XLSX | Cronograma macro do rollout por família (2023-2024) | ⭐⭐ Suporte |
| 17 | `trabalhopadrao/TPO040.pdf` | PDF | Trabalho padrão — Pino / Torno CNC | ⭐⭐⭐ Direta |
| 18 | `trabalhopadrao/TPO041.pdf` | PDF | Trabalho padrão — Cachimbo / Equiptop | ⭐⭐⭐ Direta |
| 19 | `trabalhopadrao/TPO042.pdf` | PDF | Trabalho padrão — Cachimbo / Torno CNC | ⭐⭐⭐ Direta |
| 20 | `trabalhopadrao/TPO043.pdf` | PDF | Trabalho padrão — Embalagem guarda-pó | ⭐⭐⭐ Direta |
| 21 | `Exemplo de estratificação de set up.xlsx` | XLSX | Metodologia + dados reais de setup (extrusoras, PH630, CNC20/21) | ⭐⭐ Metodológica |
| 22 | `Troca Rápida de Ferramentas.pptx` | PPTX | Treinamento SMED (71 slides) | ⭐ Metodológica |
| 23 | `workshop_pps_v1.pdf` | PDF | Workshop de sincronização da produção (120 slides, C. Panitz) | ⭐ Metodológica |
| 24 | `Antropometria_PostosdeTrabalho[1].pdf` | PDF | Tabela antropométrica para projeto de postos | ⭐ Metodológica |

> **Nota de higiene documental:** existem arquivos temporários/lixo no repositório (`Pressmatik/~$Tempos Pressmatik.xlsx`, `Pressmatik/Thumbs.db`) e uma **duplicata exata** do GBO Rev07. Recomenda-se limpeza e adoção de controle de revisão (nomes do tipo `!!Cópia de Cópia de ... Rev07` indicam ausência de versionamento formal).

---

## 4. O PROCESSO PRODUTIVO DO TD10 — FLUXO DETALHADO

### 4.1 Fluxo macro (Fluxograma Linha 10)

```
PCP
 └─ Emissão da Ordem de Produção do item casado
      │
LOGÍSTICA
 ├─ Transporte da OP até o quadro da logística
 ├─ Separação dos dois componentes (pino + cachimbo)
 ├─ A linha necessita de peças? (box vazio?)
 │     ├─ NÃO → Aguardar necessidade de abastecimento
 │     └─ SIM → Transporte dos itens casados até o box da Linha 10
 └─ Transporte do box para o pulmão da Linha 10
      │
PRODUÇÃO (TD10)
 ├─ Puxada de itens do pulmão para a linha conforme FIFO
 ├─ USINAGEM PINO            (torno CNC — TPO040)   ← GARGALO
 ├─ USINAGEM CAIXA           (torno CNC — TPO042)
 ├─ FURO E ROSCA / EQUIPTOP  (Equiptop — TPO041)
 ├─ Movimentação para o box das laminadoras
 ├─ A peça atende o requisito de priorização da Linha 10?
 │     ├─ NÃO → Aguardar / leitura das ordens de produção
 │     └─ SIM ↓
 ├─ LAMINAÇÃO DE ROSCA
 ├─ LAMINAÇÃO DE ESFERA
 ├─ MOVIMENTAÇÃO ATÉ A MONTAGEM
 ├─ MONTAGEM (bucha, graxa, pré-montagem, rolagem, laser, abraçadeiras, coifa)
 └─ EMBALAGEM (saco, selagem, cartucho, etiqueta, caixa master)
      │
 └─ Entrada na Expedição
```

**Pontos de atenção estruturais nesse fluxograma:**
- Dois pontos de espera explícitos antes mesmo da linha começar ("aguardar necessidade de abastecimento" e "aguardar até que sim" na laminação).
- O **item é "casado"** (pino + cachimbo seguem juntos), o que amarra a cadência das duas usinagens: se uma para, a outra gera WIP.
- A **priorização da laminação é por leitura de ordens**, não por puxada — fonte clássica de dessincronização (ver §18).

### 4.2 Fluxo do teste piloto (Fluxograma do Teste Piloto)

O piloto formaliza **regras de parada e qualidade** que não existiam no fluxo padrão:

```
Pagamento de Ordem
 → Logística separa as peças
 → Transporte do lote até o CNC04/CNC05
 → Usinar o pino
      ├─ Sucata? SIM → Segregar a CAIXA INTEIRA
      └─ NÃO ↓
 → Trilho cheio? SIM → INTERROMPER usinagem do pino
 → Transporte do lote para o CNC15/CNC16
 → Usinar a caixa do cachimbo
      ├─ Sucata? SIM → Segregar a caixa inteira
      └─ Pulmão cheio? SIM → INTERROMPER usinagem da caixa do cachimbo
 → Transporte do lote para o CNC46
 → Usinar furo e rosca
      ├─ Sucata? SIM → Segregar a caixa inteira
 → Transporte para as laminadoras
 → FIM DA PRIMEIRA ETAPA
```

**Máquinas nominalmente identificadas:** `CNC04/CNC05` (pino), `CNC15/CNC16` (caixa do cachimbo), `CNC46` (furo e rosca). Há duas máquinas em paralelo para pino e duas para caixa.

**O que o piloto introduz de novo:**
1. **Regra de WIP cap** ("trilho cheio" / "pulmão cheio" → interromper) — é um **CONWIP/kanban físico**, o mecanismo correto para controlar o lead time.
2. **Segregação da caixa inteira ao detectar sucata** — política de contenção de qualidade, coerente com o "Rumo ao Defeito Zero".

### 4.3 Sequência de operações elementares (conforme GBO)

As 17 atividades usadas no balanceamento de célula são:

| # | Atividade | Tempo típico (s) |
|---|---|---|
| 1 | Abastecimento Pino | 6 – 7 |
| 2 | Abastecimento Equiptop | 6,7 – 12 |
| 3 | Abastecimento Usinagem Caixa | 5,5 – 14 |
| 4 | Abastecimento Laminação | 4 – 6 |
| 5 | Laminação Rosca | 4 |
| 6 | Laminação Esfera | 4 |
| 7 | Inserir Bucha | 2 (8,22 no estado atual) |
| 8 | Adicionar Graxa | 2 |
| 9 | Abastecer a Pressmatik | 4 – 6 |
| 10 | Inserir Porca | 4,86 |
| 11 | Colocar peça no saco plástico | 4 |
| 12 | Selar o saco plástico | 4,5 |
| 13 | Abrir o cartucho | 2 |
| 14 | Etiquetar | 4 |
| 15 | Encartuchar a peça | 5,25 |
| 16 | Colocar a peça na master | 2,25 |
| 17 | Grampear a caixa | 1,67 |

Mais as atividades de **controle** acrescentadas no cenário "BALANCEADO":

| Atividade de controle | Tempo rateado (s/pç) |
|---|---|
| Inspeção Pino | 1,083 |
| Inspeção Equiptop | 1,360 |
| Inspeção Caixa (1/25) | 0,367 |
| Inspeção Caixa (1/50) | 2,040 |
| Inspeção Montagem | 6,800 |
| Preenchimento de Diário de Bordo (6 itens) | 1,0 cada = 6,0 |
| Atualizar quadro | 1,0 |
| **Total de controle** | **≈ 18,65 s/peça** |

> **Insight crítico:** quando as atividades de controle são incluídas no balanceamento, elas sozinhas representam **~18,6 s/peça** — equivalente a **mais de 60 % do takt de 30 s**. É o maior bloco isolado de carga da célula, e é justamente o alvo do projeto MeasurLink (§14).

---

## 5. DEMANDA, TAKT TIME E DIMENSIONAMENTO DE MÃO DE OBRA (GBO TERMINAL)

**Fonte:** `GBO TERMINAL.xlsx`, aba `TD10`.
**Observação do próprio documento:** *"Dados de Setup e Eficiência coletados referentes aos meses de Março e Abril."*

### 5.1 Parâmetros

| Parâmetro | Valor | Cálculo/observação |
|---|---|---|
| Linha | TD10 | — |
| Eficiência março/abril | **0,692 (69,2 %)** | medida |
| Tempo de trabalho manual total | **59,7627 s/peça** | soma dos 34 eventos |
| Demanda | **62.332 peças/mês** | — |
| Dias úteis | 27 | — |
| Tempo efetivo de operação diária | 28.800 s | 8 h |
| Demanda por turno | **769,53 peças/turno** | 62.332 ÷ 27 ÷ 3 turnos |
| **Takt time** | **37,425 s/peça** | 28.800 ÷ 769,53 |
| **Nº de operadores** | **1,597 → 2** | 59,7627 ÷ 37,425 |

Valores auxiliares na planilha: 109,09 (peças/h implícitas), 2.618,18 (peças/dia), 70.690,9 (peças/mês equivalente a 100 % de eficiência) — indicando que a linha **teria capacidade para ~70,7 mil pç/mês** se não houvesse as perdas, contra os 62,3 mil demandados.

### 5.2 Os 34 eventos cronometrados e a classificação AV / NNAV / D

| Seq | Operação | Frequência (pç) | Duração (s) | **s/peça** | Classe |
|---|---|---|---|---|---|
| 1 | Deslocamento até o palete de entrada | 450 | 5 | 0,011 | D |
| 2 | Pegar OP | 450 | 4 | 0,009 | D |
| 3 | Deslocamento até o computador | 450 | 15 | 0,033 | D |
| 4 | **Mandar imprimir os desenhos técnicos** | 450 | **600** | **1,333** | NNAV |
| 5 | Deslocamento até a impressora | 450 | — | 0 | — |
| 4b | **Preenchimento de quadro** | 80 | 90 | **1,125** | NNAV |
| 5b | Bater caixas trilho gargalo | 216 | 180 | 0,833 | D |
| 6 | **Tempo setup Pino** | 450 | **594** | **1,320** | NNAV |
| 7 | Abastecimento máquina Pino | 1 | 2 | **2,000** | **AV** |
| 8 | Desabastecimento máquina Pino | 1 | 2 | 2,000 | NNAV |
| 9 | Marcar peça com marcador industrial | 1 | 4 | 4,000 | D |
| 10 | (atividade "2") | 30 | 10 | 0,333 | NNAV |
| 11 | Inspeção Pino micrômetro com registro | 60 | 20 | 0,333 | NNAV |
| 12 | **Inspeção Pino projetor** | 60 | **300** | **5,000** | NNAV |
| 13 | Bater caixa | 18 | 30 | 1,667 | D |
| 14 | **Tempo de setup Equiptop** | 450 | **1.674** | **3,720** | NNAV |
| 15 | Inspeção Equiptop | 50 | 40 | 0,800 | NNAV |
| 16 | **Abastecimento Equiptop** | 6 | 40 | **6,667** | **AV** |
| 17 | Desabastecimento Equiptop | 6 | 15 | 2,500 | NNAV |
| 18 | **Tempo de setup Caixa** | 450 | **1.800** | **4,000** | NNAV |
| 19 | Abastecimento máquina Caixa 1 | 1 | 2 | 2,000 | **AV** |
| 20 | Abastecimento máquina Caixa 2 | 1 | 2 | 2,000 | **AV** |
| 21 | Desabastecimento máquina Caixa 1 | 1 | 2 | 2,000 | NNAV |
| 22 | Desabastecimento máquina Caixa 2 | 1 | 2 | 2,000 | NNAV |
| 23 | Inspeção Caixa cota A e E | 25 | 10 | 0,400 | NNAV |
| 24 | Inspeção Caixa demais cotas | 50 | 20 | 0,400 | NNAV |
| 25 | Bater caixas trilho de saída | 216 | 180 | 0,833 | D |
| 26 | **Tempo de deslocamento** | 1 | 10 | **10,000** | **D** |
| 27 | Preencher diário de bordo Pino | 100 | 60 | 0,600 | D |
| 28 | Preencher diário de bordo Equiptop | 100 | 60 | 0,600 | D |
| 29 | Preencher diário de bordo Caixa | 100 | 60 | 0,600 | D |
| 30 | Troca de inserto desbaste | 300 | 40 | 0,133 | NNAV |
| 31 | Troca de inserto acabamento | 550 | 180 | 0,327 | NNAV |
| 32 | Trocar ferramenta Equiptop fresa | 6.000 | 180 | 0,030 | NNAV |
| 33 | Troca de ferramenta Equiptop broca | 1.600 | 150 | 0,094 | NNAV |
| 34 | Troca de ferramenta Equiptop macho | 4.000 | 240 | 0,060 | NNAV |
| | **TOTAL** | | | **59,763** | |

### 5.3 Decomposição do tempo manual — o diagnóstico central

| Classificação | Tempo (s/pç) | % do total | Significado |
|---|---|---|---|
| **AV — Agrega Valor** | **12,667** | **21,2 %** | Abastecimento das máquinas (as 4 únicas atividades AV) |
| **NNAV — Necessário mas Não Agrega Valor** | **27,909** | **46,7 %** | Setups, inspeções, trocas de ferramenta, desabastecimentos |
| **D — Desperdício** | **19,187** | **32,1 %** | Deslocamentos, diário de bordo, bater caixas, marcação |
| **TOTAL** | **59,763** | 100 % | |

**Leitura:**
- Apenas **12,67 s de 59,76 s** (21 %) do esforço humano constrói valor.
- Se o **desperdício puro (19,19 s)** fosse eliminado, o tempo manual cairia para **40,58 s** — ainda acima do takt de 37,43 s, mas já viabilizando **1,08 operador** em vez de 1,60.
- Se além disso o **NNAV fosse reduzido pela metade** (meta realista com MeasurLink + TRF), o tempo cairia para **26,6 s**, com **0,71 operador** → **a linha operaria com 1 operador e sobra de 28 % de capacidade.**

### 5.4 Os 6 maiores consumidores de tempo

| Posição | Atividade | s/pç | % | Alavanca de melhoria |
|---|---|---|---|---|
| 1 | Deslocamento (seq. 26) | 10,00 | 16,7 % | **Layout celular** (projeto fluxo por família) |
| 2 | Abastecimento Equiptop | 6,67 | 11,2 % | AV — otimizar, não eliminar |
| 3 | Inspeção Pino projetor | 5,00 | 8,4 % | **MeasurLink** |
| 4 | Marcar peça com marcador industrial | 4,00 | 6,7 % | Marcação a laser / poka-yoke |
| 5 | Setup Caixa | 4,00 | 6,7 % | **TRF / SMED** |
| 6 | Setup Equiptop | 3,72 | 6,2 % | **TRF / SMED** |
| | **Subtotal** | **33,39** | **55,9 %** | |

> **Mais da metade do tempo manual está em 6 atividades**, todas com alavanca de melhoria já identificada e com projeto associado. Esta é a base do caso de negócio.

---

## 6. CAPACIDADE POR OPERAÇÃO E SIMULAÇÃO HORÁRIA (GBO TD10 Rev06/Rev07)

**Fontes:** `Cópia de Cópia de GBO - TD10 - Rev07.xlsx` e `GBO - TD10 - Rev06-1 - ESTUDO DE VIRADAS - DIA A DIA.xlsx`.
*(O arquivo com prefixo `!!` é duplicata exata — MD5 idêntico.)*

### 6.1 Cenário-base de capacidade (aba `Planilha3 (2)`)

| Operação | Tempo de ciclo (s) | Capacidade (pç/h) | Horas operando | Capacidade disponível (pç) |
|---|---|---|---|---|
| **PINO** | **30,3** | **118,8** | 24 | 2.851,5 |
| CAIXA (máq. 1) | 35,0 | 102,9 | 21 | 2.160,0 |
| CAIXA (máq. 2) | 35,0 | 102,9 | 0 | 0 |
| EQUIPTOP | 24,7 | 145,7 | 21 | 3.060,7 |
| MONTAGEM | 14,86 | 242,3 | 15 | 3.633,9 |
| EMBALAGEM | 19,1 | 188,5 | 21 | 3.958,1 |

**Identificação do gargalo:** com a Caixa 2 parada, a **capacidade horária mais baixa é a do PINO (118,8 pç/h)**. O documento *Projeto fluxo por família* confirma: *"Linha 10 considerado 113 pçs/hora … a 75 % de IROG no gargalo"*.

### 6.2 Cenário com 2 máquinas de caixa e montagem/embalagem turnadas (aba `Planilha3 (3)`)

| Operação | Tempo (s) | Capacidade (pç/h) | Horas operando | Capacidade disponível |
|---|---|---|---|---|
| PINO | 30,3 | 118,8 | 24 | 2.851,5 |
| CAIXA 1 | 35,0 | 102,9 | 21 | 2.160,0 |
| CAIXA 2 | 35,0 | 102,9 | 12 | 1.234,3 |
| EQUIPTOP | 24,7 | 145,7 | 21 | 3.060,7 |
| MONTAGEM 1 | 12,86 | 279,9 | 6 | 1.679,6 |
| EMBALAGEM 1 | 19,1 | 188,5 | 6 | 1.130,9 |
| MONTAGEM 2 | 13,0 | 150,0 | 13 | 1.950,0 |
| EMBALAGEM 2 | 24,02 | 149,9 | 12 | 1.798,5 |

**Totais acumulados ao fim do horizonte simulado (~39 h):**

| Etapa | Peças acumuladas |
|---|---|
| Pino | 38.675 |
| Equiptop | 37.581 |
| Caixa | 36.984 |
| Montagem | 35.892 |
| Embalagem | 35.166 |

**Perda em cascata do pino até a embalagem: 3.509 peças (−9,1 %)** — é WIP retido no sistema, não produção perdida, mas mostra a defasagem de sincronização.

### 6.3 Capacidade "limpa" (aba `Planilha4`)

| Operação | Capacidade/h | Horas produtivas | Capacidade total/dia |
|---|---|---|---|
| **PINO** | **119** | 24 | **2.856** ← menor |
| EQUIPTOP | 146 | 21 | 3.066 |
| CAIXA | 206 (2 máq.) | 21 | 4.326 |
| MONTAGEM | 150 | 21 | 3.150 |
| EMBALAGEM | 150 | 21 | 3.150 |

**Confirmação definitiva: o PINO é o gargalo (2.856 pç/dia).** A caixa, com duas máquinas, tem 51 % mais capacidade.

Comparando com a demanda: 62.332 pç/mês ÷ 27 dias = **2.308 pç/dia**. O pino entrega 2.856 pç/dia **nominal** → folga teórica de 24 %. Mas com eficiência de 69,2 %: **2.856 × 0,692 = 1.976 pç/dia**, ou seja, **déficit de 332 pç/dia (−14 %) contra a demanda**. Este é o motivo material dos atrasos.

### 6.4 Simulação horária de WIP (abas `Planilha3 (2)`, `Planilha3 (3)` e `CONSOLIDAÇÃO`)

A planilha simula hora a hora (06:00 → ciclo de 30 h) a produção de cada etapa e o WIP acumulado entre elas. Padrão identificado na aba `CONSOLIDAÇÃO` — **ciclo que se repete a cada 8 horas**:

| Hora do ciclo | WIP antes Equiptop | WIP antes Caixa | WIP antes Montagem | WIP antes Embalagem |
|---|---|---|---|---|
| h+0 | 119 | 0 | 0 | 0 |
| h+1 | 92 | 0 | 0 | 0 |
| h+2 | 65 | 0 | 0 | 0 |
| h+3 | 38 | 0 | 0 | 0 |
| h+4 | 11 | 43 | 103 | 0 |
| h+5 | 0 | 70 | 0 | **206** |
| h+6 | 0 | 86 | 103 | 18 |
| h+7 | 0 | 0 | **158** | 18 |

**Interpretação:** o WIP **oscila ciclicamente** em vez de se estabilizar — sintoma clássico de **falta de nivelamento (heijunka)** e de operação em lote com dois métodos alternados. O pico de 206 peças antes da embalagem e 158 antes da montagem são **pulmões involuntários** criados pelo desbalanceamento de horas operando entre etapas.

Na aba `Planilha3 (3)` há uma coluna **"Método" (1 ou 2)**, que alterna conforme a hora — é a troca entre o **MÉTODO 1** e o **MÉTODO 2 (quando tem WIP de caixa)** do balanceamento (§7). A planilha também calcula **"capacidade restante"** por etapa, com valores **negativos** recorrentes no Equiptop (−0,25) e na Caixa 1 (−0,14), indicando **sobrecarga sistemática** dessas duas estações no método 2.

---

## 7. BALANCEAMENTO DE OPERADORES — CENÁRIOS DE GBO

A planilha Rev07 contém **13 abas de cenário** de distribuição de trabalho. Esta é a parte mais rica do estudo.

### 7.1 ESTADO ATUAL (takt 30 s) — 5 operadores

| Atividade | Op. Pino | Op. Equiptop | Op. Caixa | Op. Laminação | Op. Montagem |
|---|---|---|---|---|---|
| Abastecimento Pino | 7,00 | | | | |
| Abastecimento Equiptop | | 6,67 | | | |
| Abastecimento Usinagem Caixa | | | 7,00 | | |
| Laminação Rosca | | | | 4,00 | |
| Laminação Esfera | | | | 4,00 | |
| Inserir Bucha | | | | | 8,22 |
| Adicionar Graxa | | | | | 2,00 |
| Abastecer Pressmatik | | | | | 4,00 |
| Inserir Porca | | | | | 4,86 |
| Colocar peça no saco | | | | | 4,00 |
| Selar o saco | | | | | 4,50 |
| Abrir o cartucho | | | | | 2,00 |
| Etiquetar | | | | | 4,00 |
| Encartuchar | | | | | 5,25 |
| Colocar na master | | | | | 2,25 |
| Grampear a caixa | 1,67 | | | | |
| **CARGA TOTAL (s)** | **8,67** | **6,67** | **7,00** | **8,00** | **41,08** |
| **Ocupação (takt 30 s)** | **28,9 %** | **22,2 %** | **23,3 %** | **26,7 %** | **137 %** ❌ |

> **O desbalanceamento do estado atual é brutal.** O operador de Montagem está com **137 % de ocupação** (41,08 s contra takt de 30 s) enquanto os 4 operadores de usinagem estão com **22 % a 29 %**. Há **~75 s de ociosidade por ciclo** distribuídos em 4 pessoas enquanto a 5ª é o gargalo humano.

### 7.2 BALANCEADO (takt 30 s) — 5 operadores, **com** atividades de controle

| Atividade | Op. Pino | Op. Equiptop | Op. Caixa | Op. Laminação | Op. Montagem |
|---|---|---|---|---|---|
| Abastecimento Pino | 7,00 | | | | |
| Abastecimento Equiptop | 12,00 | | | | |
| Abastecimento Usinagem Caixa | | | 7,00 | | |
| Laminação Rosca / Esfera | | | | 4,00 + 4,00 | |
| Inserir Bucha | | | 2,00 | | |
| Adicionar Graxa | | | 2,00 | | |
| Abastecer Pressmatik | | | | | 4,00 |
| Inserir Porca | | | | 4,86 | |
| Saco / Selagem | | | | | 4,00 + 4,50 |
| Abrir cartucho | | | | | 2,00 |
| Etiquetar | | | | 4,00 | |
| Encartuchar / Master | | | | | 5,25 + 2,25 |
| Grampear a caixa | 1,67 | | | | |
| **Inspeção Pino** | 1,08 | | | | |
| **Inspeção Equiptop** | | 1,36 | | | |
| **Inspeção Caixa (1/25)** | | | 0,37 | | |
| **Inspeção Caixa (1/50)** | | | 2,04 | | |
| **Inspeção Montagem** | | | | 6,80 | |
| **Diário de bordo 1 e 2** | 1,00 + 1,00 | | | | |
| **Diário de bordo 3 e 4** | | | 1,00 + 1,00 | | |
| **Diário de bordo 5 e 6** | | | | 1,00 + 1,00 | |
| **Atualizar quadro** | | | 1,00 | | |
| **CARGA TOTAL (s)** | **23,75** | **1,36** | **16,41** | **25,66** | **22,00** |
| **Ocupação (takt 30 s)** | **79,2 %** | **4,5 %** ❌ | **54,7 %** | **85,5 %** | **73,3 %** |

Há uma variante **BALANCEADO (2)** que corrige parcialmente, devolvendo o abastecimento do Equiptop (12 s) e a inserção de porca (4,86 s) ao Operador Equiptop:

| | Op. Pino | Op. Equiptop | Op. Caixa | Op. Laminação | Op. Montagem |
|---|---|---|---|---|---|
| **CARGA TOTAL (s)** | **11,75** | **18,22** | **14,41** | **18,80** | **16,00** |
| **Ocupação (takt 30 s)** | **39,2 %** | **60,7 %** | **48,0 %** | **62,7 %** | **53,3 %** |

> **BALANCEADO (2) é claramente o melhor cenário de 5 operadores**: carga total 79,18 s, desvio máximo de ocupação entre 39 % e 63 %. Mesmo assim, com ocupação média de **52,8 %**, **a célula sobra mão de obra** — comporta ser operada com **3 operadores** (79,18 ÷ 30 = 2,64).

### 7.3 Cenários de 4 operadores (MÉTODO 1, MÉTODO 2, NOVO LAYOUT) — takt 28 s

| Cenário | Op1 | Op2 | Op3 | Op4 | **Soma** | Ocupação máx. |
|---|---|---|---|---|---|---|
| **MÉTODO 1** | 6,00 | 19,50 | 12,86 | 19,17 | **57,53** | 69,6 % (Op2) |
| **MÉTODO 2** (com WIP de caixa) | 6,00 | 20,00 | 13,00 | 24,03 | **63,03** | 85,8 % (Op4) |
| **NOVO LAYOUT** (Rev06) | 12,00 | 23,00 | 14,86 | 19,17 | **69,03** | 82,1 % (Op2) |
| **NOVO LAYOUT (2)** (Rev06) | 12,00 | 20,00 | 13,00 | 24,03 | **69,03** | 85,8 % (Op4) |

**Detalhamento do MÉTODO 1** (o mais enxuto, 57,53 s):

| Atividade | Op1 | Op2 | Op3 | Op4 |
|---|---|---|---|---|
| Abastecimento Pino | 6,00 | | | |
| Abastecimento Equiptop | | 12,00 | | |
| Abastecimento Usinagem Caixa | | 5,50 | | |
| Inserir Bucha | | 2,00 | | |
| Adicionar Graxa | | | 2,00 | |
| Abastecer Pressmatik | | | 6,00 | |
| Inserir Porca | | | 4,86 | |
| Saco plástico | | | | 4,00 |
| Abrir cartucho | | | | 2,00 |
| Etiquetar | | | | 4,00 |
| Encartuchar | | | | 5,25 |
| Colocar na master | | | | 2,25 |
| Grampear a caixa | | | | 1,67 |
| **Total** | **6,00** | **19,50** | **12,86** | **19,17** |

**Diferença MÉTODO 1 vs MÉTODO 2:** quando existe WIP de caixa disponível, o abastecimento da usinagem de caixa sobe de 5,5 s para 11 s (manuseio do WIP) e a inserção de porca migra do Op3 para o Op4, elevando a carga total em **+5,5 s (+9,6 %)**. **O WIP, além de custar lead time, custa 5,5 s de trabalho extra por peça.**

### 7.4 Cenários de 3 operadores — takt 28 s

| Cenário | Op1 | Op2 | Op3 | **Soma** | Ocupação máx. |
|---|---|---|---|---|---|
| **NOVO LAYOUT – 3 OP CEN 2** | 22,86 | 23,42 | 27,00 | **73,28** | **96,4 %** ⚠ |
| **NOVO LAYOUT CENÁRIO 3 OP** | 14,92 | 26,50 | 23,86 | **65,28** | **94,6 %** ⚠ |
| **CENÁRIO 1** | 15,17 | 23,86 | 20,00 | **59,03** | **85,2 %** ✅ |
| **CENÁRIO 2** | 15,17 | 19,86 | 24,00 | **59,03** | **85,7 %** ✅ |
| **CENÁRIO 3** | 15,17 | 20,86 | 26,00 | **62,03** | **92,9 %** ⚠ |

**Detalhamento do CENÁRIO 1 (melhor cenário de 3 operadores):**

| Atividade | Op1 | Op2 | Op3 |
|---|---|---|---|
| Abastecimento Pino | 7,00 | | |
| Abastecimento Equiptop | | 10,00 | |
| Abastecimento Usinagem Caixa | | | 14,00 |
| Abastecimento Laminação | | 4,00 | |
| Inserir Bucha | | | 2,00 |
| Adicionar Graxa | | | 2,00 |
| Abastecer Pressmatik | | 5,00 | |
| Inserir Porca | | 4,86 | |
| Colocar peça no saco plástico | | 4,00 | |
| Selar o saco plástico | 4,50 | | |
| Abrir o cartucho | 2,00 | | |
| Etiquetar | 4,00 | | |
| Encartuchar | 5,25 | | |
| Colocar na master | 2,25 | | |
| Grampear a caixa | 1,67 | | |
| **Total** | **15,17** | **23,86** | **20,00** |
| **Ocupação (takt 28 s)** | **54,2 %** | **85,2 %** | **71,4 %** |

> **Recomendação de balanceamento:** o **CENÁRIO 1 com 3 operadores** é viável e deixa 14,8 % de folga no posto mais carregado — margem razoável para absorver variabilidade. Comparado ao estado atual de 5 operadores, representa **redução de 2 operadores por turno (−40 % de MOD na célula)**. ⚠ **Porém esses cenários não incluem as atividades de controle (18,65 s/pç).** Com controle incluído, 3 operadores só são viáveis **após** o MeasurLink eliminar a inspeção manual.

### 7.5 Resumo comparativo de todos os cenários

| Cenário | Nº Op | Takt (s) | Carga total (s) | Ocupação média | Ocupação máx. | Inclui controle? |
|---|---|---|---|---|---|---|
| ESTADO ATUAL | 5 | 30 | 71,42 | 47,6 % | **137 %** ❌ | Não |
| BALANCEADO | 5 | 30 | 89,18 | 59,5 % | 85,5 % | ✅ Sim |
| BALANCEADO (2) | 5 | 30 | 79,18 | 52,8 % | 62,7 % | ✅ Sim |
| MÉTODO 1 | 4 | 28 | 57,53 | 51,4 % | 69,6 % | Não |
| MÉTODO 2 | 4 | 28 | 63,03 | 56,3 % | 85,8 % | Não |
| NOVO LAYOUT | 4 | 28 | 69,03 | 61,6 % | 85,8 % | Não |
| **CENÁRIO 1** | **3** | **28** | **59,03** | **70,3 %** | **85,2 %** | Não |
| CENÁRIO 2 | 3 | 28 | 59,03 | 70,3 % | 85,7 % | Não |
| CENÁRIO 3 | 3 | 28 | 62,03 | 73,8 % | 92,9 % | Não |
| 3 OP CEN 2 | 3 | 28 | 73,28 | 87,2 % | 96,4 % ❌ | Não |

---

## 8. PERDAS DE DISPONIBILIDADE — O ACHADO MAIS CRÍTICO

**Fonte:** aba `PERDAS DE DISPONIBILIDADE` (Rev06 e Rev07).

| Atividade | Tempo unitário (s) | Repetições/turno | **Tempo total (s)** | % do total |
|---|---|---|---|---|
| Inspeção caixa (1/50) | 102 | 20 | 2.040 | 7,2 % |
| Inspeção caixa (1/25) | 29 | 40 | 1.160 | 4,1 % |
| Inspeção Equiptop (1/50) | 106 | 20 | 2.120 | 7,5 % |
| **Inspeção montagem** | **1.000** | **7** | **7.000** | **24,8 %** |
| Inspeção pino (1/60) | 60 | 17 | 1.020 | 3,6 % |
| **Virada 1** | **3.600** | **1** | **3.600** | **12,8 %** |
| **Virada 2** | **3.600** | **1** | **3.600** | **12,8 %** |
| Preencher diário de bordo | 60 | 48 | 2.880 | 10,2 % |
| Preencher quadro | 60 | 8 | 480 | 1,7 % |
| Setup Pino | 720 | 1 | 720 | 2,6 % |
| Setup Equiptop | 1.758 | 1 | 1.758 | 6,2 % |
| Setup Caixa | 1.800 | 1 | 1.800 | 6,4 % |
| **TOTAL DE PERDAS** | | | **28.178 s** | 100 % |
| **Tempo disponível por turno** | | | **26.400 s** | |
| **RAZÃO PERDAS/DISPONÍVEL** | | | **1,0673 → 106,7 %** | |

### 8.1 Interpretação

> **As paradas "planejadas" consomem 106,7 % do tempo disponível do turno.** Matematicamente, a linha **não cabe** no turno: se todas as paradas fossem executadas conforme a norma, **não sobraria um único segundo para produzir**.

Isso tem três consequências diretas e verificáveis:

1. **Explica a eficiência de 69,2 %** — é a eficiência que resta depois que parte das paradas acontece (e parte, presumivelmente, é suprimida informalmente pelos operadores).
2. **Cria um "sistema informal"**: inspeções são puladas, diários são preenchidos em lote no fim do turno, viradas são postergadas. Isso é exatamente o anti-padrão descrito no material de PPCP (§18): *"nasce um PCP informal (verbal) baseado em listas críticas"*.
3. **Torna o padrão não auditável** — o trabalho padrão (TPO040-043) descreve a operação, mas o tempo total prescrito é fisicamente impossível.

### 8.2 Pareto das perdas — onde atacar

| Bloco | Tempo (s) | % | Projeto que ataca |
|---|---|---|---|
| **Inspeções (5 tipos)** | **13.340** | **47,3 %** | **MeasurLink / Projeto F4** |
| **Viradas (2)** | **7.200** | **25,6 %** | **Fluxo por família / nivelamento** |
| **Setups (3)** | **4.278** | **15,2 %** | **TRF / SMED** |
| Registros (diário + quadro) | 3.360 | 11,9 % | MeasurLink (digitalização) |
| **TOTAL** | **28.178** | 100 % | |

- **A inspeção da montagem (1.000 s × 7 = 7.000 s) sozinha é 24,8 % de todas as perdas.** É o alvo isolado de maior retorno.
- **MeasurLink + digitalização de registros ataca 59,2 % das perdas** (16.700 s). Se eliminasse metade disso (8.350 s), a razão cairia de 106,7 % para **75,1 %**, liberando ~25 % de tempo produtivo.
- **TRF nos 3 setups** (4.278 s): uma redução SMED típica de 50 % devolve 2.139 s (8,1 % do turno).

### 8.3 Aba `Planilha2` — visão alternativa de paradas

| Parada | Tempo (s) |
|---|---|
| Setup Pino | 1.800 |
| **Virada** | **10.800** |
| Inspeção Pino | 1.600 |
| Inspeção Caixa | 1.600 |
| Inspeção Equiptop | 1.600 |
| Inspeção Laminação | 1.600 |
| Montagem | 1.600 |
| **Total** | **20.600** (contra 25.200 s de referência) |

Nesta visão, a **virada vale 10.800 s (3 h)** e sozinha é **52,4 % das paradas**. ⚠ Há divergência entre as duas abas (3.600×2 = 7.200 s vs 10.800 s) — ver §21.

### 8.4 Aba `Planilha1` — comparação de produtividade

| | Amostra A | Amostra B |
|---|---|---|
| Medição 1 | 631 | 2.062 |
| Medição 2 | 1.317 | 2.047 |
| Medição 3 | 1.561 | 2.109 |
| Medição 4 | 1.485 | 1.663 |
| **Média** | **1.248,5** | **1.970,25** |
| **Razão A/B** | **63,4 %** | |

Esses números são compatíveis com **peças produzidas por turno**: um cenário atual (~1.248 pç) contra um cenário de referência/proposto (~1.970 pç) — **um potencial de +57,8 % de produção** com a mesma estrutura. A razão de 63,4 % é muito próxima da eficiência medida de 69,2 %, reforçando a consistência do diagnóstico.

---

## 9. MONTAGEM / EMBALAGEM — CRONOANÁLISE E YAMAZUMI

### 9.1 GBO Montagem — tempos médios por posto

**Fonte:** `GBO Montagem.xlsx` (abas `Planilha1` e `Médias - Tempos`, com 12 cronometragens por atividade).

| Posto | Atividade | Tempo médio (s) | Nº de cronometragens |
|---|---|---|---|
| Operador 1 | Colocar Bucha + Graxa | **5,88** | 12 (média bruta 3,43 + graxa) |
| Operador 2 | Pré-Montagem | **6,18** | 12 |
| Operador 3 | Rolagem | **5,74** | 12 |
| Operador 4 | Marcação a Laser | **5,31** | 12 |
| Operador 5 | Colocação de Abraçadeira | **5,89** | 9 |
| Operador 6 | Inserção da Coifa | **9,67** | 12 |
| **Operador 7** | **Colocação de Abraçadeira (2)** | **12,98** ← gargalo | 11 |
| Operador 8 | Ensacar | **3,67** | 6 |
| Operador 9 | Embalagem | **8,04** | 12 |
| Operador 10 | Etiquetagem da Caixa | **1,83** | 12 |
| Operador 9 | Embalagem Grande (21 peças) | **34,61** (= 1,65 s/pç) | 3 |

**Análise:**
- **Soma dos tempos: 65,19 s** distribuídos em 10 postos → tempo médio por posto **6,52 s**.
- **Gargalo: Colocação de Abraçadeira (2) — 12,98 s**, ou seja **99 % acima da média**. Esse posto sozinho define o ritmo da montagem.
- **Variabilidade do gargalo é altíssima**: as 11 medições vão de **7,50 s a 19,75 s** (amplitude de 163 %, desvio-padrão ≈ 3,8 s). Isso indica **falta de padronização ou dificuldade ergonômica/dispositivo inadequado**.
- **Desbalanceamento:** o posto mais rápido (etiquetagem, 1,83 s) é **7,1× mais rápido** que o gargalo. Com linha balanceada ao gargalo (12,98 s), a **perda de balanceamento é de 65,19 ÷ (10 × 12,98) = 50,2 %** — metade da capacidade de mão de obra é ociosidade.
- **Capacidade atual da montagem ao gargalo:** 3.600 ÷ 12,98 = **277 pç/h**.
- **Com balanceamento perfeito em 5 postos de 13,04 s:** mesma capacidade com **metade dos operadores**.

**Variabilidade por posto (das tabelas de cronometragem):**

| Atividade | Mín (s) | Máx (s) | Amplitude | Observação |
|---|---|---|---|---|
| Colocar Bucha + Graxa | 2,50 | 4,80 | 92 % | Aceitável |
| Pré-Montagem | 5,50 | 8,00 | 45 % | Boa |
| Rolagem | 5,00 | 8,00 | 60 % | Boa |
| Marcação a Laser | 4,75 | 6,00 | 26 % | Excelente |
| Marcação a Laser (c/ buffer) | 3,25 | 4,50 | 38 % | **Buffer reduz tempo em 31 %** |
| Colocação de Abraçadeira | 4,35 | 8,75 | 101 % | Alta |
| Inserção da Coifa | 8,00 | 13,25 | 66 % | Alta |
| **Colocação de Abraçadeira (2)** | **7,50** | **19,75** | **163 %** | ❌ Crítica |
| Ensacar | 3,00 | 4,75 | 58 % | Boa |
| Embalagem | 6,74 | 11,00 | 63 % | Alta |
| Etiquetagem | 1,25 | 2,50 | 100 % | Tempos pequenos |
| Caixa grande (21 pç) | 28,47 | 42,25 | 48 % | Média |

> **Achado relevante:** a Marcação a Laser **com buffer** tem média de **3,67 s contra 5,31 s sem buffer** — **redução de 31 %**. Isso é evidência direta e quantificada de que **desacoplar postos com pequenos pulmões reduz o tempo de ciclo** na montagem. Replicável nos demais postos.

### 9.2 Ferramenta GBO + YAMAZUMI — Montagem MTD 335272

**Fonte:** `Ferramenta GBO + YAMAZUMI - Rev1 (Manipulação 4 operadores).xlsm`
**Elaborador:** David Teixeira — Engenharia | **Data:** 03/03/2025 | **Método:** análise de vídeo

#### 9.2.1 Parâmetros do estudo

| Parâmetro | Valor |
|---|---|
| Tempo disponível | 1.260 min/dia (21 h) · 31.500 min/mês |
| Dias úteis | 25 dias/mês |
| **Demanda** | **230.000 peças/mês = 9.200 peças/dia** |
| **Takt Time** | **8,217 s** |
| Eficiência necessária | 78 % |
| Capacidade necessária | 561,7 pç/h · 11.794,9 pç/dia |

> ⚠ Note a **diferença de ordem de grandeza**: este estudo trata da **montagem da família inteira** (230 mil pç/mês), enquanto o GBO TERMINAL trata do **TD10 isoladamente** (62,3 mil pç/mês). São escopos complementares, não contraditórios.

#### 9.2.2 Estado ATUAL — 5 postos

| Posto | Operação | Movimentações | Tméd (s) | Coef. fadiga | **Tméd ajustado (s)** | Ocupação (takt 8,22 s) |
|---|---|---|---|---|---|---|
| OP1 | Fechamento + Gravação + Pré-montagem | 6 | 6,165 | 4,76 % | **6,473** | 78,8 % ← **gargalo** |
| OP2 | Aplicação do Guarda-pó | 7 | 6,180 | 4,76 % | **6,489** | 79,0 % |
| OP3 | Embalagem saco plástico | 4 | 3,593 | 4,76 % | **3,772** | 45,9 % |
| OP4 | Cartucho | 7 | 7,464 | 4,76 % | **7,837** | 95,4 % |
| OP5 | Master | 22 | 5,590 | 13,04 % | **6,428** | 78,2 % |
| | **TOTAL** | **46** | | | **31,00** | |

**Indicadores do estado atual:**

| Indicador | Valor |
|---|---|
| Gargalo | **6,473 s** |
| Lead Time (soma dos ciclos) | **28,99 s** |
| Capacidade instalada | **556,1 pç/h = 11.678,8 pç/dia** |
| Nº de postos teórico (pelo takt) | 3,53 → 4 |
| Nº de postos teórico (pelo gargalo) | 4,48 → **5** |
| Eficiência | **88,2 %** |
| Tempo necessário | 16h32min (contra 21h disponíveis) |

**Decomposição AV / Necessário / Desperdício (estado atual):**

| Posto | Agrega valor (s) | Necessário (s) | Desperdício (s) | % desperdício |
|---|---|---|---|---|
| OP1 | 0,465 | 4,415 | 1,285 | 20,9 % |
| OP2 | 0,570 | 5,610 | 0,000 | 0 % |
| OP3 | 1,389 | 1,004 | 1,200 | 33,4 % |
| OP4 | 1,938 | 2,437 | 3,089 | **41,4 %** ❌ |
| OP5 | 0,000 | 4,295 | 1,294 | 23,2 % |
| **TOTAL** | **4,362** | **17,761** | **6,868** | |
| **%** | **15,0 %** | **61,3 %** | **23,7 %** | |

> **Apenas 15 % do tempo da montagem agrega valor.** O OP4 (Cartucho) é o mais crítico: **41,4 % de desperdício** e ocupação de 95,4 %.

#### 9.2.3 Estado PROPOSTO — 4 postos (eliminando atividades)

Atividades marcadas como **"Manter? Não"** (eliminadas):

| Posto | Atividade eliminada | Tempo (s) |
|---|---|---|
| OP1 | Esperar para retirar a peça | 0,500 |
| OP4 | Arrumar cartuchos fechados na mesa | 0,600 |
| OP4 | Disponibiliza o cartucho fechado para a próxima operação | 1,289 |
| OP4 | Grampear as abas da parte superior da caixa | 0,059 |
| OP4 | Grampear parte de baixo da caixa | 0,082 |
| OP4 | Guardar o grampeador (×2) | 0,102 |
| OP4 | Pegar grampeador e posicionar (×2) | 0,107 |
| OP4 | Pegar pincel, abrir e marcar a etiqueta, fechar e guardar | 0,200 |
| | **TOTAL ELIMINADO** | **≈ 2,94 s** |

> **Toda a operação de grampeamento manual foi eliminada** — sinal de que foi previsto um **selador/fita automática** ou caixa auto-montável. Também foi eliminado o **pincel atômico de conferência**, substituído presumivelmente por verificação visual ou sistema.

**Novo arranjo proposto (OP4 absorve o posto MASTER, eliminando o OP5):**

| Posto | Operação | Movim. | Tméd (s) | Coef. fadiga | **Tméd ajustado (s)** | Ocupação (takt 8,22 s) |
|---|---|---|---|---|---|---|
| OP1 | Fechamento + Gravação + Pré-montagem | 6 | 5,300 | 2,91 % | **5,459** | 66,4 % |
| OP2 | Aplicação do Guarda-pó | 7 | 5,520 | 2,91 % | **5,686** | 69,2 % |
| OP3 | Embalagem saco plástico | 4 | 3,578 | 4,76 % | **3,757** | 45,7 % |
| **OP4** | **Cartucho + Master** | 7 | 9,867 | 2,91 % | **10,163** | **123,7 %** ❌ |
| | **TOTAL** | | | | **25,06** | |

**Indicadores do estado proposto:**

| Indicador | Atual | **Proposto** | Variação |
|---|---|---|---|
| Gargalo "oficial" | 6,473 s | **5,459 s** | **−15,7 %** |
| Lead Time | 28,99 s | **24,26 s** | **−16,3 %** |
| Capacidade instalada | 556 pç/h | **659 pç/h** | **+18,6 %** |
| Capacidade dia | 11.679 pç | **13.849 pç** | **+18,6 %** |
| Nº de postos (takt) | 3,53 → 4 | **3,79 → 4** | — |
| Eficiência | 88,2 % | **94,6 %** | **+6,4 p.p.** |
| Tempo necessário | 16h32min | **13h57min** | **−2h35min** |
| Nº real de postos | **5** | **4** | **−1 operador** |

**Decomposição AV / Necessário / Desperdício (proposto):**

| | Atual | Proposto | Variação |
|---|---|---|---|
| Agrega valor | 4,362 s (15,0 %) | 4,242 s (17,3 %) | +2,3 p.p. |
| Necessário | 17,761 s (61,3 %) | 16,346 s (66,7 %) | −1,42 s |
| **Desperdício** | **6,868 s (23,7 %)** | **3,677 s (15,0 %)** | **−46,5 %** ✅ |

> ⚠ **ALERTA TÉCNICO IMPORTANTE:** o cenário proposto declara gargalo de 5,459 s, mas o **OP4 (Cartucho + Master) fica com 10,163 s — 23,7 % ACIMA do takt de 8,217 s**. A proposta **não é executável como está**: consolidar Cartucho e Master em um único operador cria um novo gargalo pior que o original. É preciso:
> - redistribuir atividades do OP4 para OP3 (que tem apenas 45,7 % de ocupação, com **4,46 s de folga**); ou
> - automatizar a montagem/fechamento da caixa master; ou
> - manter 5 postos com redistribuição (o cenário BALANCEADO do GBO).
>
> **Transferindo ~2,5 s de atividades do OP4 para o OP3**, chega-se a OP3 = 6,26 s e OP4 = 7,66 s — **ambos abaixo do takt**, com 4 postos viáveis. Esta é a correção recomendada.

#### 9.2.4 As 46 atividades da montagem (estado atual, completo)

| Posto | Atividade | MOP | Classe | Tméd (s) | Freq. | Tméd ajust. (s) |
|---|---|---|---|---|---|---|
| OP1 | Pegar o cachimbo com bucha com a mão direita | TMP | NECESSÁRIO | 1,650 | 1 | 1,650 |
| OP1 | Levar o cachimbo até a graxeira | TMP | **DESPERDÍCIO** | 0,785 | 1 | 0,785 |
| OP1 | **Aplicar a graxa** | TMP | **AGREGA VALOR** | 0,465 | 1 | 0,465 |
| OP1 | Unir cachimbo com pino | TMP | NECESSÁRIO | 0,915 | 1 | 0,915 |
| OP1 | Esperar para retirar a peça | TMP | **DESPERDÍCIO** | 0,500 | 1 | 0,500 |
| OP1 | Retira a peça processada e abastece com a nova | TMP | NECESSÁRIO | 1,850 | 1 | 1,850 |
| OP2 | Retirar peça do dispositivo e abastecer | TOM | NECESSÁRIO | 1,600 | 1 | 1,600 |
| OP2 | Pegar limitador (esq.) + peça montada (dir.) | TOM | NECESSÁRIO | 1,070 | 1 | 1,070 |
| OP2 | Unir peça montada com limitador | TOM | NECESSÁRIO | 0,670 | 1 | 0,670 |
| OP2 | Pegar um guarda-pó com a mão esquerda | TOM | NECESSÁRIO | 0,670 | 1 | 0,670 |
| OP2 | **Unir peça montada com guarda-pó** | TOM | **AGREGA VALOR** | 0,570 | 1 | 0,570 |
| OP2 | Inspeção + Lançamento | TOM | NECESSÁRIO | 120,0 | 150 | 0,800 |
| OP2 | Movimentação de componentes | TOM | NECESSÁRIO | 120,0 | 150 | 0,800 |
| OP3 | Pega saco e abre (esq.) + peça montada (dir.) | TOM | NECESSÁRIO | 0,930 | 1 | 0,930 |
| OP3 | **Coloca peça e porca no saco e libera** | TMO | **AGREGA VALOR** | 1,389 | 1 | 1,389 |
| OP3 | Pega um "punhado" de porcas com a mão direita | TMO | NECESSÁRIO | 1,100 | 15 | 0,073 |
| OP3 | Abrir saco plástico e disponibilizar sobre a mesa | TMO | **DESPERDÍCIO** | 120,0 | 100 | 1,200 |
| OP4 | Pega cartucho, leva até a esquerda e abre | TOM | NECESSÁRIO | 0,887 | 1 | 0,887 |
| OP4 | Pega o termo e coloca dentro do cartucho | TOM | NECESSÁRIO | 1,017 | 1 | 1,017 |
| OP4 | **Pega a peça e coloca dentro do cartucho** | TOM | **AGREGA VALOR** | 1,938 | 1 | 1,938 |
| OP4 | Fecha o cartucho | TOM | NECESSÁRIO | 0,533 | 1 | 0,533 |
| OP4 | Disponibiliza cartucho fechado p/ próxima op. | TOM | **DESPERDÍCIO** | 1,289 | 1 | 1,289 |
| OP4 | Arrumar cartuchos fechados na mesa | TOM | **DESPERDÍCIO** | 6,000 | 10 | 0,600 |
| OP4 | Abastecer a mesa de cartuchos | TOM | **DESPERDÍCIO** | 120,0 | 100 | 1,200 |
| OP5 | Pega a caixa fechada debaixo da mesa | TOM | NECESSÁRIO | 0,900 | 18 | 0,050 |
| OP5 | Coloca a caixa em cima da mesa e abre | TOM | NECESSÁRIO | 1,030 | 18 | 0,057 |
| OP5 | Dobrar abas da caixa master | TOM | **DESPERDÍCIO** | 1,800 | 18 | 0,100 |
| OP5 | Pegar grampeador e posicionar | TOM | **DESPERDÍCIO** | 0,730 | 18 | 0,041 |
| OP5 | Grampear parte de baixo da caixa | TOM | NECESSÁRIO | 1,470 | 18 | 0,082 |
| OP5 | Guardar o grampeador | TOM | **DESPERDÍCIO** | 1,000 | 18 | 0,056 |
| OP5 | Virar a caixa e abrir as abas de cima | TOM | **DESPERDÍCIO** | 2,330 | 18 | 0,129 |
| OP5 | Abastecer a caixa com cartuchos | TOM | NECESSÁRIO | 16,00 | 18 | 0,889 |
| OP5 | Fechar as abas da parte de cima da caixa | TOM | NECESSÁRIO | 2,470 | 18 | 0,137 |
| OP5 | Pegar o grampeador e posicionar | TOM | NECESSÁRIO | 1,200 | 18 | 0,067 |
| OP5 | Grampear as abas da parte superior | TOM | NECESSÁRIO | 1,070 | 18 | 0,059 |
| OP5 | Guardar o grampeador | TOM | **DESPERDÍCIO** | 0,830 | 18 | 0,046 |
| OP5 | Virar a caixa para colar etiqueta | TOM | **DESPERDÍCIO** | 0,930 | 18 | 0,052 |
| OP5 | Pegar a etiqueta, descolar e aplicar na caixa | TOM | NECESSÁRIO | 4,870 | 18 | 0,271 |
| OP5 | Pegar pincel, abrir, marcar etiqueta, fechar, guardar | TOM | **DESPERDÍCIO** | 3,600 | 18 | 0,200 |
| OP5 | Largar a caixa para a próxima posição | TOM | **DESPERDÍCIO** | 1,060 | 18 | 0,059 |
| OP5 | Levar caixas fechadas acumuladas para o palete | TOM | NECESSÁRIO | 120,0 | 90 | 1,333 |
| OP5 | Colar etiqueta no cartucho | TOM | NECESSÁRIO | 0,950 | 1 | 0,950 |
| OP5 | Recolher o fim das etiquetas e colocar no lixo | TOM | **DESPERDÍCIO** | 2,500 | 50 | 0,050 |
| OP5 | Colocar mais cartuchos na mesa e organizar | TOM | **DESPERDÍCIO** | 13,93 | 50 | 0,279 |
| OP5 | Recortar etiquetas e organizar p/ aplicar | TOM | **DESPERDÍCIO** | 14,17 | 50 | 0,283 |
| OP5 | Imprimir etiquetas | TOM | NECESSÁRIO | 180,0 | 450 | 0,400 |
| | **TOTAL GERAL** | | | | | **28,991 s** |

*(MOP = classificação de movimento: TMP = Trabalho Máquina-Parada; TOM = Trabalho Operador-Máquina; TMO = Trabalho Manual-Operador.)*

**Observações relevantes:**
- O **OP5 (Master) concentra 22 das 46 atividades (48 %)** mas apenas **5,59 s (19 % do tempo)** — é um posto de **altíssima fragmentação e manipulação**, com coeficiente de fadiga de **13,04 %** (quase 3× o dos demais postos, que é 4,76 %). **Risco ergonômico documentado.**
- **Operações de etiquetagem somam 5 atividades distintas** (imprimir, colar no cartucho, recortar, recolher restos, aplicar na caixa) totalizando **1,982 s/pç** — **candidato óbvio a aplicador automático de etiquetas**.
- **"Levar as caixas fechadas acumuladas para o palete" custa 120 s a cada 90 peças (1,333 s/pç)** — resolve-se com trilho roletado de saída (exatamente o que o projeto de fluxo por família está comprando).

---

## 10. CÉLULA PRESSMATIK — ESTUDO DE CENÁRIOS

**Fonte:** `Pressmatik/Tempos Pressmatik.xlsx`

A Pressmatik é a prensa de inserção da célula (bucha/porca). Foram cronometrados **4 cenários** de arranjo de trabalho.

### 10.1 CENÁRIO 1 (13 ciclos cronometrados)

| Elemento | Tempo médio (s) | Amplitude observada |
|---|---|---|
| Operação Pressmatik | **10,955** | 10,00 – 13,58 |
| Porca | **5,707** | 3,72 – 10,60 |
| Saquinho | **7,613** | 5,89 – 9,61 |
| Caixinha | **7,716** | 6,90 – 8,87 |
| Etiqueta (média separada) | 4,600 | 3,14 – 6,63 |
| Bucha (média separada) | 8,220 | — |
| Ciclo montagem master | 0,830 | — |
| Ciclo finalização master | 1,234 | — |
| **TEMPO TOTAL DE OPERAÇÃO** | **46,875 s** | |

### 10.2 CENÁRIO 3 (6 ciclos)

| Elemento | Tempo médio (s) |
|---|---|
| Bucha | 8,218 |
| Operação Pressmatik | **2,707** ← queda de 75 % |
| Porca | 4,855 |
| Saquinho | 8,503 |
| Caixinha | **15,802** ← subiu muito |
| Ciclo montagem master | 0,830 |
| Ciclo finalização master | 1,234 |
| **TEMPO TOTAL** | **42,149 s** |

### 10.3 CENÁRIO 4 (10 ciclos)

| Elemento | Tempo médio (s) |
|---|---|
| Bucha | 8,916 |
| Operação Pressmatik | **2,457** |
| Saquinho | 9,779 |
| Caixinha | 12,941 |
| Ciclo montagem master | 0,830 |
| Ciclo finalização master | 1,234 |
| **TEMPO TOTAL** | **36,157 s** |

### 10.4 CENÁRIO 5 (6 ciclos) — **o melhor**

| Elemento | Tempo médio (s) |
|---|---|
| Operação Pressmatik | 9,753 |
| Saquinho | 10,222 |
| Caixinha | 12,220 |
| Ciclo montagem master | 0,830 |
| Ciclo finalização master | 1,234 |
| **TEMPO TOTAL** | **34,259 s** |

### 10.5 COMPARAÇÃO FINAL

| | Cenário 1 | Cenário 3 | Cenário 4 | **Cenário 5** |
|---|---|---|---|---|
| **Tempo de ciclo (s)** | 46,88 | 42,15 | 36,16 | **34,26** |
| **Entrega (pç/h)** | 76,8 | 85,4 | 99,6 | **105,1** |
| **Ganho vs. Cenário 1** | — | +11,2 % | +29,6 % | **+36,8 %** |

| Métrica de fechamento | Valor |
|---|---|
| **Melhor tempo de ciclo** | **34,26 s** |
| **Takt alvo** | **31,50 s** |
| **GAP** | **2,76 s (8,8 % acima do takt)** ⚠ |

> **Conclusão da Pressmatik:** a evolução do Cenário 1 ao 5 trouxe **36,8 % de ganho de produtividade** (76,8 → 105,1 pç/h), mas **ainda existe um gap de 2,76 s contra o takt de 31,5 s**. O cenário 5 entrega 105 pç/h contra as ~114 pç/h necessárias (3.600 ÷ 31,5).
>
> **Onde buscar os 2,76 s faltantes:** o elemento **"Caixinha" (12,22 s) é o maior do cenário 5** e tem histórico de variação enorme entre cenários (7,72 → 15,80 → 12,94 → 12,22 s). Há sinais de 3 medições no Cenário 5 de **28,83 / 27,60 / 32,46 s** (tempos totais individuais), mostrando variabilidade de ±8 % no ciclo completo. **Padronizar o encartuchamento resolve o gap.**

**Medições da Master (registro complementar):**

| | Montagem master | Finalização master |
|---|---|---|
| Medição 1 | 14,91 s | 23,60 s |
| Medição 2 | 14,96 s | 20,83 s |
| **Média** | **14,935 s** | **22,215 s** |
| **Rateado por peça (18 pç/caixa)** | **0,830 s** | **1,234 s** |

---

## 11. LAMINADORAS — OPERAÇÃO A JUSANTE

**Fonte:** `GBO - Laminadoras.xlsx`

### 11.1 Parâmetros

| Parâmetro | Valor |
|---|---|
| **IROG** | **0,70 (70 %)** |
| Nº de setups por dia | 3 |
| **Demanda dia** | **8.500 peças** |
| Demanda rosca macho | 1.275 peças (15 % da demanda) |

### 11.2 Tempos de ciclo

| Operação | Tempo de ciclo (s) | Capacidade a 100 % (pç/h) | Capacidade a 70 % IROG (pç/h) |
|---|---|---|---|
| **Rosca** | 6 | 600 | 420 |
| **Esfera** | 4 | 900 | 630 |
| **Macho** | 10 | 360 | 252 |

### 11.3 Cenário A — 3 operadores

| Operador | Operação c/ IROG (s) | Setup (s) | **Horas utilizadas** | Ocupação (24 h) |
|---|---|---|---|---|
| Operador 1 (Rosca) | 72.857,1 | 7.200 | **22,24 h** | **92,7 %** |
| Operador 2 (Esfera) | 48.571,4 | 3.600 | **14,49 h** | 60,4 % |
| Operador 3 (Rosca Macho) | 18.214,3 | 8.100 | **7,31 h** | 30,5 % |
| **Total** | | | **44,04 h** | |

### 11.4 Cenário B — 2 operadores (recomendado pela planilha)

| Operador | Operação c/ IROG (s) | Setup (s) | **Horas utilizadas** | Ocupação (24 h) |
|---|---|---|---|---|
| Operador 1 (Rosca) | 72.857,1 | 7.200 | **22,24 h** | **92,7 %** |
| Operador 2 (Esfera + Rosca Macho) | 66.785,7 | 11.700 | **21,80 h** | **90,8 %** |
| **Total** | | | **44,04 h** | |

> **Conclusão das laminadoras:** o **Cenário B elimina 1 operador** consolidando esfera + rosca macho, com ambos os operadores em ~91-93 % de ocupação. ⚠ **Essa ocupação é alta demais para operação robusta** — não deixa margem para variabilidade, quebras ou absenteísmo. Recomenda-se **primeiro reduzir o setup** (que consome 7.200 a 11.700 s/dia, equivalente a **2 a 3,25 h/operador**) via TRF e só então consolidar.
>
> **Potencial TRF nas laminadoras:** reduzir os setups em 50 % liberaria **1 a 1,6 h por operador por dia**, trazendo a ocupação para ~85 %, faixa saudável.

---

## 12. MAPA DE FLUXO DE VALOR (MFV 335074) E ANÁLISE SHINGO

### 12.1 MFV — Terminal Direção Celta (335074), Rev. 00

**Fonte:** `MFV - Terminal de Direção 335074 - Rev. 00.xls`

#### 12.1.1 Cadeia mapeada

```
Pino (C607176)              Cachimbo (C606099)
Recebimento 1,5 ton          Forn.: Eletroforja
                             Entrega semanal · Lead time 20 dias
        │                            │
        ├─ Área das serras e cisalhadoras
        │   (Cisalhadora · setup 15 min · 2.200 pç/lote)
        │
        ├─ Metal Brill e proximidades (beneficiamento)
        │   ├─ Desengraxe   (1.100 pç/batelada)
        │   ├─ Jateamento   (Jato de granalha · 750 pç)
        │   └─ Fosfato e Sabão (1.100 pç/batelada)
        │
        ├─ Estoque do Recebimento e Intermediário (TKS)
        │
        ├─ Área da Conformação (Prensa TM 315 · 2 pç/ciclo · 2.200 pç)
        │   └─ Inspeção de dureza (1 pç por caixa · 315 peças)
        │
        ├─ Área de Usinagem (Torno · 1.000 pç · medição e leitura de perfil 1 pç/50)
        │
        ├─ Usinagem da Rosca
        │
        ├─ Área da Laminadora (1.000 pç)
        │
        └─ Montagem final (LMTG) — 544 pç
            ├─ MTG-bucha superior + pino   (Prensinha)
            ├─ MTG-bucha inferior          (Prensinha)
            ├─ Fechamento                  (Prensinha)
            ├─ Gravação                    (Prensinha)
            ├─ MTG limitador               (Manual)
            ├─ MTG anel (guarda-pó e graxa)(Manual)
            ├─ Embala saco plástico        (Manual)
            ├─ Selagem                     (Prensinha)
            ├─ Embalar na caixa individual (Manual)
            └─ Embalar 20 pç/caixa         (Manual)
                 │
            Aguarda expedição · Paleteira → EXPEDIÇÃO
```

**Tempos de montagem final cronometrados no MFV:** 4,33 / 4,00 / 5,00 / 4,60 / 5,70 / 5,30 / 3,00 / 1,00 / 4,50 / 2,00 s — **total 39,43 s**, com tempo total de espera acumulado de **17.915,7 s** no posto.

#### 12.1.2 Resultados quantitativos do MFV

**Cenário A — CONSIDERANDO BENEFICIAMENTO COMO VALOR AGREGADO:**

| Categoria | Segundos | Horas | Dias | % do Lead Time |
|---|---|---|---|---|
| **Espera por processamento** | 796.200 | **221,17** | 9,215 | **66,19 %** |
| Transporte | 701,6 | 0,195 | 0,008 | 0,06 % |
| **Processamento (VA)** | 25.630,3 | **7,120** | 0,297 | **2,13 %** |
| Inspeção | 30.000 | 8,333 | 0,347 | 2,49 % |
| **Espera de lote** | 350.344,8 | **97,318** | 4,055 | **29,13 %** |
| **LEAD TIME TOTAL** | **1.202.876,7** | **334,13 h** | **13,92 dias** | 100 % |

**Cenário B — NÃO CONSIDERANDO BENEFICIAMENTO COMO VA:**

| Categoria | Segundos | Horas | Dias | % |
|---|---|---|---|---|
| Espera por processamento | 796.200 | 221,17 | 9,215 | 66,19 % |
| Transporte | 701,6 | 0,195 | 0,008 | 0,06 % |
| **Processamento (VA)** | 1.030,3 | **0,286** | 0,012 | **0,086 %** |
| Inspeção | 30.000 | 8,333 | 0,347 | 2,49 % |
| Espera de lote | 350.344,8 | 97,318 | 4,055 | 29,13 % |
| **LEAD TIME TOTAL** | **1.178.276,7** | **327,30 h** | **13,64 dias** | 100 % |

**Distância total percorrida pelo material: 870 metros.**

#### 12.1.3 Leitura do MFV

> **Para entregar ~7 horas de processamento efetivo, o produto 335074 passa 334 horas (14 dias) no sistema.** A razão de eficiência de fluxo é de **2,13 %** — e se o beneficiamento (que é terceirizado e em batelada) não for contado como valor agregado, cai para **0,086 %**.

**Onde está o lead time:**

| Bloco | Horas | % | Causa raiz |
|---|---|---|---|
| **Espera por processamento** | 221,2 | 66,2 % | Filas entre operações, falta de sincronização, ordens empurradas |
| **Espera de lote** | 97,3 | 29,1 % | Lotes de 1.000 a 2.200 peças; bateladas de beneficiamento de 750-1.100 pç |
| Inspeção | 8,3 | 2,5 % | Inspeções de dureza e perfil, medição ponto a ponto |
| Processamento | 7,1 | 2,1 % | O único tempo que o cliente paga |
| Transporte | 0,2 | 0,06 % | Irrelevante em tempo (mas 870 m de movimentação) |

**As duas alavancas são evidentes:**
1. **Reduzir tamanho de lote** ataca diretamente as 97,3 h de espera de lote (29 %). O projeto de fluxo por família já define lotes de **450 peças** (metade do lote do teste de julho) — se aplicado, a espera de lote cairia proporcionalmente.
2. **Sincronizar o fluxo (puxada/CONWIP)** ataca as 221,2 h de espera por processamento (66 %). O fluxograma do teste piloto já define as regras ("trilho cheio → interromper").

**Simulação de impacto (estimativa):**

| Cenário | Espera de lote | Espera por processamento | Lead time estimado | Redução |
|---|---|---|---|---|
| Atual (lote ~2.000) | 97,3 h | 221,2 h | **334,1 h (13,9 d)** | — |
| Lote 450 pç | ~21,9 h | 221,2 h | **258,7 h (10,8 d)** | **−22,6 %** |
| Lote 450 + CONWIP (−50 % espera) | ~21,9 h | ~110,6 h | **148,1 h (6,2 d)** | **−55,7 %** |

#### 12.1.4 Pontos críticos anotados no próprio MFV

O documento contém observações manuscritas reveladoras:
- *"Para onde vão as outras 1.200 pcs???"* — **evidência de perda de rastreabilidade de WIP**.
- *"pro estoque intermediário"* — resposta encontrada, confirmando acúmulo não planejado.
- *"Esperando OP"* (no estoque do recebimento) — **material parado aguardando ordem**, típico de PCP empurrado.
- *"Aguardando OP"* (frente ao estoque de componentes) — repetição do mesmo padrão a jusante.
- *"leva 2 dias para entregar 500 pcs, depois entrega 500 pcs/dia"* (Eletroforja) — **perfil de entrega do fornecedor que cria espera de lote na entrada**.
- *"Setup 15 minutos"* (cisalhadora) — único setup quantificado no MFV.

### 12.2 Análise SHINGO — AV / NAV (Terminal)

**Fonte:** `SHINGO - AV NAV.xlsx`, aba `SHINGO - F3`

**Porcentagem de valor agregado (Terminal):**

| Símbolo / Atividade | Agrega valor? | TAV (min) | TNAV (min) | % do Lead Time |
|---|---|---|---|---|
| Estoque M.P. | N | — | 0 | 0 % |
| **Transporte** | N | — | 6 | 0,0295 % |
| **Esperando Processo** | N | — | **19.980** | **98,19 %** |
| **PROCESSANDO** | **S** | **1,43** | — | **0,00703 %** |
| **Esperando Lote** | N | — | **360** | **1,769 %** |
| Inspeção | N | — | 0 | 0 % |
| Estoque Produto | N | — | 0 | 0 % |
| **TOTAL** | | **1,43 min** | **20.346 min** | |

| Indicador | Valor |
|---|---|
| **Lead Time Total** | **20.347,43 min** |
| **Lead Time Total** | **339,12 h** |
| **Lead Time Total** | **14,13 dias** |
| **% valor agregado** | **0,00703 %** |

Parâmetros de contagem registrados (colunas d/h/t/e/l/P): 13 / 18 / 2 / 19.800 / — / 32 na primeira linha; 5/2/—/300/24 na segunda; 3/2/180/—/18 na terceira; 1/—/60/4 na quarta; —/6/19.980/360/4 na quinta. Totais de ocorrências: **86 eventos**, dos quais apenas **1,43 min** processando. Valores complementares registrados: 39 / 6 / 18 / **63**.

> **Convergência dos dois métodos:** MFV diz **13,92 dias**; Shingo diz **14,13 dias**. Diferença de 1,5 % — **os dois mapeamentos independentes confirmam o mesmo lead time**. A diferença de % de VA (2,13 % vs 0,007 %) vem de critério: o MFV conta todas as operações de transformação (incluindo beneficiamento, 7,1 h), o Shingo conta apenas o processamento estrito da peça (1,43 min).

---

## 13. TRABALHO PADRÃO (TPO040 A TPO043)

### 13.1 TPO040 — PINO / TERMINAL — Torno CNC

| Campo | Conteúdo |
|---|---|
| **Produto** | PINO / TERMINAL |
| **Equipamento** | TORNO CNC |
| **Tempo de ciclo** | **TD10/TD20/TD30 = tempo máquina + 7 s** · **TD40 = tempo máquina + 4 s** |
| **EPIs** | Luva de corte, luva antivibratória, sapato, protetor auricular, óculos |

| Seq | Descrição | Tempo homem (s) | Tempo ciclo (s) |
|---|---|---|---|
| 1 | Pegar peça na caixa de entrada | 2 | |
| 2 | Abertura automática de porta | 2 | |
| 3 | Aperta pedal e retira peça usinada | 2 | |
| 4 | Coloca peça bruta e aperta pedal de fechamento | 2 | |
| 5 | Aciona ciclo start | 1 | |
| 6 | Fechamento automático de porta | 2 | |
| 7 | **Ciclo de usinagem** | | **15** |
| 8 | Retirar cavaco da peça pronta (quando houver) | 4 | |
| 9 | Marcação da peça | 2 | |
| 10 | Coloca peça pronta na caixa de saída | 2 | |
| | | | **14** (ciclo total) |
| 11 | Realizar troca de inserto na frequência estipulada pelo programa CNC | | |
| 12 | A inspeção é realizada conforme **PC001** | | |
| 13 | **Peça de setup pintada de VERDE** na região do arraste | 2 | |
| 14 | **Peça de inspeção pintada de AMARELO** na região do arraste | 2 | |
| 15 | Colocar separadores nas caixas quando houver mais de uma OP no trilho | 3 | |
| 16 | **Pintar a peça de sucata com a pinta VERMELHA** | | |

> **Sistema de gestão visual por cor já padronizado: VERDE = setup, AMARELO = inspeção, VERMELHO = sucata.**

### 13.2 TPO041 — CACHIMBO / TERMINAL — EQUIPTOP

| Campo | Conteúdo |
|---|---|
| **Produto** | CACHIMBO / TERMINAL |
| **Equipamento** | EQUIPTOP |
| **Tempo de ciclo** | **TEMPO MÁQUINA / 6** (máquina processa 6 peças por pallet) |
| **EPIs** | Luva Maxidry, sapato, protetor auricular, óculos |

| Seq | Descrição | Tempo (s) |
|---|---|---|
| 1 | Abrir dispositivo de fixação | 1 |
| 2 | Abrir a porta | 2 |
| 3 | Limpar cavacos do dispositivo (durante abertura da garra) | 6 |
| 4 | Retirar peças prontas | 8 |
| 5 | Colocar peças na caixa de saída | 2 |
| 6 | Pegar peças brutas na caixa de entrada | 3 |
| 7 | **Posicionar peças no dispositivo** | **20** ← maior elemento |
| 8 | Fechar dispositivo | 1 |
| 9 | Aguardar fechamento das garras | 9 |
| 10 | Fechar a porta | 2 |
| 11 | Travar a porta para liberar giro do pallet | 1 |
| 12 | **Realizar inspeção conforme PC033** | **65** |
| 13 | Troca de inserto, ponteira da broca e macho conforme **NPU0013** | — |
| 14 | Peça de setup pintada de VERDE (1 por pallet) na região do pescoço | 2 |
| 15 | Peça de inspeção e troca de ferramenta pintada de AMARELO (1 por pallet) | 2 |
| 16 | Separadores nas caixas quando houver mais de uma OP no trilho | 2 |
| 17 | Pintar peça de sucata com pinta vermelha | 2 |
| | **CICLO DE ABASTECIMENTO COM INSPEÇÃO E REGISTRO** | **128 s** |

> **O ciclo completo do Equiptop é de 128 s, dos quais a inspeção (PC033) consome 65 s — 50,8 %.** É a confirmação pontual do diagnóstico: **metade do trabalho do operador do Equiptop é inspeção**. Alvo direto do MeasurLink.

### 13.3 TPO042 — CACHIMBO / TERMINAL — Torno CNC

| Campo | Conteúdo |
|---|---|
| **Tempo de ciclo** | **TEMPO MÁQUINA + 8 s** |
| **EPIs** | Luva de corte, luva antivibratória, sapato, protetor auricular, óculos |

| Seq | Descrição | Tempo (s) |
|---|---|---|
| 1 | Pegar peça na caixa de entrada | 1 |
| 2 | Abertura automática de porta e da pinça | 2 |
| 3 | Retirar peça pronta e colocar peça bruta | 2 |
| 4 | Aperta pedal | 1 |
| 5 | Aciona ciclo start | 1 |
| 6 | Fechamento automático de porta | 2 |
| 7 | Pegar peça na caixa de entrada para abastecer máquina | 2 |
| 8 | **Deslocamento até a máquina** | **2** |
| 9 | Abertura automática de porta e da pinça | 2 |
| 10 | Retirar peça pronta e colocar peça bruta | 3 |
| 11 | Aciona ciclo start | 1 |
| 12 | Fechamento automático de porta | 2 |
| 13 | Coloca a peça no dispositivo | 1 |
| 14 | Quando completar o dispositivo, marcar as peças | 4 |
| 15 | Colocar a peça na caixa de saída | 1 |
| 16 | Peça de setup pintada de VERDE na região frontal da caixa (forjado) | 2 |
| 17 | Peça de inspeção pintada de AMARELO na região frontal da caixa | 2 |
| 18 | Separadores nas caixas quando houver mais de uma OP no trilho | 3 |
| 19 | Pintar peça de sucata com pinta vermelha | 2 |

> **Confirma a operação de 2 máquinas em paralelo (CNC15/CNC16)** — os passos 1-6 são a máquina A e os passos 7-12 a máquina B, com deslocamento entre elas.

### 13.4 TPO043 — EMBALAGEM GUARDA-PÓ CAIXA DE DIREÇÃO

| Campo | Conteúdo |
|---|---|
| **Documento** | TPO043-01 · "Sem validade se impresso" |
| **Rev. 0** | 13/11/2023 — Elaboração — David Teixeira / Maicon Lemos / José Guedes |
| **Rev. 1** | 01/04/2024 — Inclusão das imagens de referência |
| **Componentes** | Guarda-pó, saco plástico, etiqueta master, etiqueta saco plástico |

| # | Operação |
|---|---|
| 1 | Iniciar OP conforme **IT 215**; imprimir etiquetas da OP conforme **IT 147** |
| 2 | Posicionar sacos plásticos e etiquetas de forma organizada |
| 3 | Colar etiqueta no saco plástico e disponibilizar para a operação seguinte |
| 4 | Inserir no furo inferior do guarda-pó (maior diâmetro) um **termo de garantia** |
| 5 | Pegar saco plástico com a mão esquerda pelo lado da "boca" |
| 6 | Abrir a "boca" do saco plástico com a mão esquerda |
| 7 | Colocar o saco aberto na parte chanfrada do **tubo embalador** |
| 8 | Segurar o saco no tubo e passar o guarda-pó com termo por dentro |
| 9 | **Realizar a selagem na seladora — garantir a qualidade da selagem** |
| 10 | Abastecer a caixa master **de 2 em 2 guarda-pós**, inspecionando a presença da etiqueta |
| 11 | Fechar a caixa master e fazer check com **pincel atômico**, garantindo a etiqueta grande |

> **Conexão com o Yamazumi:** a operação 11 ("check com pincel atômico") é exatamente a atividade **"Pegar pincel, abrir e marcar a etiqueta, fechar e guardar novamente" (3,6 s)** classificada como **DESPERDÍCIO** e marcada para eliminação no cenário proposto. **Eliminá-la exige revisar o TPO043.**

### 13.5 Documentos de referência citados (não presentes no repositório)

| Documento | Função |
|---|---|
| **PC001** | Plano de controle — inspeção do pino |
| **PC033** | Plano de controle — inspeção do Equiptop (65 s) |
| **NPU0013** | Norma de troca de inserto/broca/macho do Equiptop |
| **IT 215** | Instrução de trabalho — abertura de ordem de produção |
| **IT 147** | Instrução de trabalho — impressão de etiquetas |
| **FO021** | Formulário de registro de inspeção em papel (a ser eliminado pelo MeasurLink) |

---

## 14. PROJETO DE CAPABILIDADE / MEASURLINK (PROJETO F4)

**Fonte:** `01 - PROJETO DE CAPABILIDADE TD10 (MeasurLink) - atualizado 06.08.24.pptx`
**Responsáveis:** Paulo Frosi · Dieferson Antunes

### 14.1 Objetivo declarado

> *"Implementar um sistema de medição online avançado para inspeção de peças fabricadas na usinagem, proporcionando controle estatístico do processo em tempo real, aumento de eficiência devido à maior disponibilidade do operador, precisão nas medições, eliminação do uso de registros em papel, bem como a **redução de 30 % da sucata operacional** gerada na linha TD10, assegurando que as peças sejam fabricadas corretamente na primeira vez, servindo como base para os projetos **"F4"** e **"Rumo ao Defeito Zero"**."*

### 14.2 Mudança de modelo

| Modelo ATUAL | Modelo PROPOSTO |
|---|---|
| Abertura do registro de inspeção (papel FO021) | Abertura automática no MeasurLink |
| Inspeção com instrumentos analógicos | Inspeção com instrumentos digitais com transmissão de dados |
| Registro manual dos dados | Registro automático |
| Fechamento manual | Fechamento no sistema |
| Arquivamento físico (caixas de arquivo) | Arquivamento digital |

### 14.3 Fases de implementação

| Fase | Escopo | Prazo |
|---|---|---|
| **1ª Fase** | Efetivação na linha **TD10 Gargalo** | **15 dias** após liberação do CAPEX |
| **2ª Fase** | Implementação na **linha TD10 completa** | **90 dias** após liberação do CAPEX |
| **3ª Fase** | Demais células, conforme avanço do Projeto **"F4"** | Conforme avanço |

> **Nota estratégica:** a Fase 1 ataca **exatamente o gargalo (pino)** — decisão correta pela Teoria das Restrições: toda hora ganha no gargalo é hora ganha no sistema.

### 14.4 Investimento TD10 — detalhamento

**Piloto gratuito:** 45 dias sem custo, sistema fornecido pelo representante Mitutoyo.

**Software, hardware e infraestrutura:**

| Item | Qtd | Valor (R$) |
|---|---|---|
| Pacote com 2 licenças | 1 | 30.000,00 |
| Equipamentos e instrumentos de medição | 1 | 14.979,16 |
| Computador completo | 1 | 5.000,00 |
| Leitor de código de barras | 1 | 300,00 |
| Cabo HDMI | 1 | 40,00 |
| Ponto de rede | 1 | 2.000,00 |
| Licença CAL do servidor | 1 | 1.800,00 |
| Mesa com suporte para TV | 1 | 500,00 |
| Nobreak | 1 | 600,00 |
| Ponto de energia | 1 | 1.200,00 |
| **TOTAL** | | **R$ 56.419,16** |

**Instrumentos de medição — FASE 1 TD10:**

| Qtd | Instrumento | Custo (R$) |
|---|---|---|
| 1 | Paquímetro 150 | 3.046,54 |
| 1 | Micrômetro ext. 0–25 | 3.278,52 |
| 1 | Micrômetro ext. 25–50 | 4.104,83 |
| 1 | Paquímetro 300 | 4.549,27 |
| | **TOTAL** | **R$ 14.979,16** |

**Suporte técnico:**

| Fornecedor | Modalidade | Custo |
|---|---|---|
| Mitutoyo | Presencial | R$ 180/h + deslocamento |
| Mitutoyo | **Remoto** | **Gratuito por tempo indeterminado** |
| 3D Metrologia | Presencial | R$ 150/h + deslocamento |
| 3D Metrologia | **Remoto** | **Gratuito por tempo indeterminado** |

> Suporte do **software** direto com a Mitutoyo; suporte de **ferramental** direto com a 3D Metrologia.

**Requisitos de sistema:**

| Categoria | Requisito |
|---|---|
| **SGBD** | Microsoft SQL Server 2014 / 2016 / 2017 (Standard ou Enterprise) |
| **SO** | Windows 8 (exceto RT) e Windows 10 (exceto Mobile/IoT), 32 e 64 bits |
| **Processador** | 1 GHz ou superior (x86 ou x64) |
| **RAM** | 4 GB (32 bits) ou 8 GB (64 bits) |
| **Disco** | 16 GB (32 bits) ou 20 GB (64 bits) |
| **Vídeo** | DirectX 9 com WDDM 1.0 ou superior |
| **Mídia** | DVD-ROM (opcional) |

### 14.5 Ganhos TANGÍVEIS — linha TD10

**Base de cálculo: 06/2023 a 06/2024**

| Ganho | Tipo | Fator | Valor (R$) | **Valor considerado (R$)** |
|---|---|---|---|---|
| Redução do nº de sucata operacional > 1 peça (TD10) | Ganho pontual | 1 | 2.170,00 | **2.170,00** |
| Aderência ao MPS — perdas com desvio e retrabalho (Gargalo) | Risco evitado | 0,25 | 246.576,00 | **61.644,00** |
| Aderência ao MPS — perdas com sucata operacional (Gargalo) | Ganho mensal constante | 1 | 418,00 | **418,00** |
| Aderência ao MPS — perdas com desvios e retrabalho (Equiptop e caixa) | Risco evitado | 1 | 88.660,00 | **88.660,00** |
| Aderência ao MPS — perdas com sucata operacional (Equiptop e caixa) | Risco evitado | 1 | 11.528,00 | **11.528,00** |
| Redução de custos com papel físico (**FO021**) | Ganho mensal constante | 1 | 42,12 | **42,12** |
| Redução de caixas de arquivamento | Ganho mensal constante | 1 | 2,60 | **2,60** |
| Aderência ao MPS — estudos de capabilidade (perda de 24 h para 4 h) | Ganho pontual | 1 | 105.600,00 | **105.600,00** |
| Redução no custo de calibração externa | Ganho mensal constante | 2 | 109,50 | **219,00** |
| | | | **TOTAL** | **R$ 270.283,72** |

**Decomposição por natureza:**

| Natureza | Valor (R$) | Observação |
|---|---|---|
| **Ganhos pontuais** | **107.770,00** | Sucata (2.170) + capabilidade (105.600) |
| **Riscos evitados** | **161.832,00** | Desvios/retrabalhos e sucata no gargalo e Equiptop/caixa |
| **Ganhos mensais constantes** | **681,72 /mês** | Sucata gargalo (418) + papel (42,12) + arquivo (2,60) + calibração (219) |

**Payback (estimativa a partir dos dados):** considerando apenas os **ganhos pontuais de R$ 107.770,00** contra o investimento de R$ 56.419,16, o **payback é inferior a 1 ano já no primeiro ciclo**, com ROI de **+91 %**. Incluindo riscos evitados, o retorno é de **4,8× o investimento**.

### 14.6 Base de cálculo detalhada (06/2023 a 06/2024)

**a) Redução de 50 % de sucatas > 1 peça:**

| | Peças | Valor unitário | Total |
|---|---|---|---|
| Total de sucatas | 376 | | |
| Pino | 57 | R$ 3,60 | R$ 205,20 |
| Cachimbo | 131 | R$ 15,00 | R$ 1.965,00 |
| | | **TOTAL** | **R$ 2.170,20** |

**b) Aderência ao MPS — faturamento não realizado por sucatas > 1 peça:**

| | Peças | Valor unitário | Total |
|---|---|---|---|
| Total de sucatas | 376 | | |
| Pino | 114 | R$ 44,00 | R$ 5.016,00 |
| Cachimbo | 262 | R$ 44,00 | R$ 11.528,00 |
| | | **TOTAL** | **R$ 16.544,00** |

**c) Aderência ao MPS — faturamento fora do prazo por retrabalhos e desvios:**

| | Peças | Valor unitário | Total |
|---|---|---|---|
| Total de peças | 9.425 | | |
| Pino | 1.401 | R$ 44,00 | R$ 61.644,00 |
| Cachimbo | 575 | R$ 44,00 | R$ 25.300,00 |
| | | **TOTAL** | **R$ 86.944,00** |

**d) Redução de máquina parada por estudos de capabilidade:**

| | Atual | Proposto |
|---|---|---|
| **Tempo médio de parada** | **24 h** | **4 h** |
| **Impacto no gargalo** | **3.072 peças** | **512 peças** |
| Produção horária do gargalo | 128 pç/h | 128 pç/h |
| **Impacto no faturamento** | **− R$ 135.168** | **− R$ 22.528** |
| **GANHO (por máquina)** | | **R$ 112.640** |

> ⚠ Note que aqui o gargalo é referido como **128 pç/h**, enquanto o GBO Rev07 aponta **119 pç/h** e o projeto de fluxo por família **113 pç/h a 75 % de IROG**. Ver §21 (inconsistências).

### 14.7 Ganhos INTANGÍVEIS

1. **Capabilidade do processo em tempo real** (gestão visual).
2. **Rapidez na tomada de decisão** baseada em resultados imediatos (análise estatística).
3. **Melhoria na exatidão das medições** — mitigação de erros de transcrição e interpretação, via instrumentos digitais com transmissão de dados.
4. **Redução de 50 % no número de instrumentos utilizados.**
5. **Disponibilidade dos dados em tempo real** — informação documentada, requisito de norma (IATF/ISO).
6. **Alerta na tela e disparo de e-mail** quando uma peça medida estiver fora de tolerância.
7. **Possibilidade de bloqueio de máquina** quando uma peça estiver fora de tolerância **ou quando a medição não for realizada no período estipulado**.
8. **Eficiência operacional** — elimina digitação manual e processamento de dados, com **redução de 3 minutos no tempo de medição (setup e troca de OP)**.

### 14.8 Riscos declarados

| Risco | Natureza |
|---|---|
| Gestão da mudança | Organizacional |
| Má utilização dos equipamentos | Operacional |
| Falha na coleta de dados ou perda por falta de energia | Técnico (mitigado pelo nobreak) |
| Custo adicional para interligação software ↔ máquina (bloqueio do CNC) | Financeiro |
| Interligação de outros meios de medição ao sistema (outros fabricantes) | Técnico |

### 14.9 Projeto F4 — mapa de investimento macro da fábrica

| Família | Células | Investimento por célula (R$) | **Subtotal (R$)** |
|---|---|---|---|
| **Terminal** | **TD10** | **56.419,16** | |
| | TD20 | 41.419,16 | |
| | TD30 | 41.419,16 | |
| | TD40 | 41.419,16 | **180.676,64** |
| **Pivô** | PA10, PA20, PA30, PA40, PC10, PC20, PC30, PC40, JS10, JS20 (parcial) | 36.869,89 (maioria) / 41.639,27 | **336.598,35** |
| **Axial** | JS10, JS20 | 36.869,89 | **106.206,70** |
| **Tirante/Freio** | TE10/1 | 39.915,87 | |
| | TE10/2 | 46.406,87 | **86.322,74** |
| **Conformação** | — | — | **137.203,00** |
| | | **VALOR TOTAL ESTIMADO** | **R$ 847.000,00** |

**Legenda de status:** Em andamento · Não iniciado · Conceito de célula não implementado.
**Observação do documento:** *"Sem cotação com outros fornecedores."*

> O **TD10 é a célula de maior investimento unitário (R$ 56.419,16)** porque inclui o pacote de licenças e o servidor — as demais aproveitam a infraestrutura. **O TD10 é o investimento habilitador de toda a fábrica.**

### 14.10 Árvore de benefícios declarada

```
MEASURLINK – TD10
    ├─ Reduzir 30 % do percentual de sucata na linha TD10
    ├─ Mudança de cultura
    ├─ Fazer Certo na Primeira Vez
    ├─ Eficiência operacional
    ├─ Redução no tempo de não agregação de valor (registro FO021)
    └─ Indústria 4.0
         ↓
    RUMO AO DEFEITO ZERO  ·  F4
```

---

## 15. PROJETO "FLUXO POR FAMÍLIA" — PILOTO DA CÉLULA TERMINAL

**Fonte:** `Projeto fluxo por familia (piloto celula terminal).xlsx`, `lista de materiais.xlsx`, `fluxo macro.xlsx`

### 15.1 As 10 premissas do projeto (texto integral da aba `Premissas`)

| # | Premissa |
|---|---|
| 1 | Escolheu-se as **linhas 10 e 40** para lote piloto em função de não necessitarem movimentação nas máquinas de caixas, e as Equiptops somente seriam viradas |
| 2 | Considerou-se para efeito do orçamento o **menor tempo de parada da linha**. Por este motivo, 4 ligações elétricas e 4 pneumáticas serão novas |
| 3 | Considerou-se que o layout das linhas piloto **não sofrerá grandes alterações** após sua validação com a produção |
| 4 | Considerou-se o conceito de **LINHA em vez de CÉLULA**, em função da organização atual dos equipamentos |
| 5 | Não foram consideradas visões do futuro layout oficial, em função do **menor custo de implantação possível** (a entrada ideal deste fluxo é perpendicular ao fluxo proposto) |
| 6 | Considerado **lotes de 450 peças** (metade do lote do teste feito em julho) em função de **minimizar o lead time** |
| 7 | Nº de paletes: **2 na entrada e 2 na saída** da linha, para linhas 10 e 40 |
| 8 | Considerando **1 dia para processo fluxo abaixo na linha (laminação)** e **1 dia de proteção no gargalo** (menos 2 paletes já de entrada da linha) |
| 9 | **Linha 10: 113 pç/hora** · Linha 40: 80 pç/hora · **a 75 % de IROG no gargalo** |
| 10 | **Máquinas da linha 20 serão agora máquinas da linha 10** |

### 15.2 Dimensionamento de buffers

| Tipo de buffer | Descrição | **Linha 10** | Linha 40 |
|---|---|---|---|
| **Time buffer** | Espaço de paletes na logística (1 m²) | **3 paletes (1.350 pç)** | 2 (900 pç) |
| **Time buffer** | Espaço de paletes na entrada da linha (1 m²) | **2 paletes (900 pç)** | 2 (900 pç) |
| **Space buffer** | Espaço de trilho (nº de KLT) | **9 KLT (162 pç)** | 9 (162 pç) |
| **Buffer** | Palete na saída da linha / entrada da laminação | **5 paletes (2.250 pç)** | 4 (1.800 pç) |
| **Buffer** | Montagem | **5 paletes (2.250 pç)** | 4 (1.800 pç) |
| | **TOTAL DE WIP DIMENSIONADO** | **6.912 peças** | 2.142 peças |

**Parâmetros físicos:**

| Parâmetro | Valor |
|---|---|
| Lote estimado | **450 pç por lote/OP** |
| Quantidade por KLT | **18 pç/KLT** |
| Necessidade de caixas de pino | **25 por lote/palete casado** |
| Necessidade total de caixas de pino | **503 caixas BIN NR3** |
| Peso por caixa | 15 kg |
| Kits por caixa | 18 |
| Modelo de caixa | **KLT 4314 — 400 × 300 × 148 mm (E)** |
| **Autonomia do space buffer** | **162 pç (9 cx × 18 casados)** |
| Peso máximo por metro linear projetado | **45 kg** |

**Dimensões dos trilhos roletados:**

| | Sem rodízio | Com rodízio |
|---|---|---|
| Altura de entrada | 0,72 m | **0,885 m** |
| Altura de saída | 0,65 m | **0,785 m** |
| Largura | 0,40 m | 0,40 m |
| Comprimento | 3 m | 3 m |

> **Nota ergonômica:** altura de entrada de **0,885 m** está compatível com a recomendação antropométrica de superfície de trabalho em pé (§17). Altura de saída de 0,785 m também está em faixa aceitável.

### 15.3 Orçamento de materiais

**Preços unitários levantados (24/09/2022):**

| Material | Especificação | Preço (R$) | Fornecedor |
|---|---|---|---|
| Cantoneira | 2" × 1/4 × 6 m (ou 2" × 3/16 × 6 m) | 224,51 | ArcelorMittal |
| Rodízio giratório | PU 100 mm até 300 kg — SCHIOPPA GL414-PE | 160,90 | Loja do Mecânico |
| Tubo | 40 × 40 × 3,00 mm × 6 m | 209,91 | ArcelorMittal |
| Trilho roletado flow rack | Carga 65 kg/m × 3 m | 163,71 | IPC |
| Caixa pino | BIN NR3 azul | 1,67 | CCP |
| Caixa pino | BIN NR4 azul | 2,88 | CCP |
| Tubo PVC | 150 mm × 6 m | 170,90 | Superproatacado (Amanco) |

**Composição de custo — trilho Viemar roletado de 3 m:**

| Material | Qtd | Valor (R$) |
|---|---|---|
| Cantoneira | 4 | 898,04 |
| Rodízio giratório | 4 | 643,60 |
| Tubo | 1 | 209,91 |
| Trilho roletado flow rack | 2 | 327,42 |
| **TOTAL MP** | | **2.078,97** |
| MO (Sr. Paulo — interna) | | — |

**Composição de custo — trilho Viemar roletado de 4 m:**

| Material | Qtd | Valor (R$) |
|---|---|---|
| Cantoneira | 5 | 1.122,55 |
| Rodízio giratório | 4 | 643,60 |
| Tubo | 2 | 419,82 |
| Trilho roletado flow rack | 3 | 491,13 |
| **TOTAL MP** | | **2.677,10** |

**Caixas de pino:** 503 × BIN NR3 = **R$ 840,01**

### 15.4 Instalações e serviços

| Instalação | Valor por máquina (R$) | Orçamentista | Observação |
|---|---|---|---|
| Elétrica | Sem valores | Manutenção | Alexandre ver com Anderson (MO); Lucimar estimar material; Thiago Queiroz orçar |
| **Pneumática** | **3.500** | PNX (material e MO) | Valores orçados para a linha Axial (Vicente) |
| **Nivelamento Centro** | **3.000** | Allservice Caxias do Sul | Confirmar com Anderson usando a Oliveira (mais barato) |
| Nivelamento Tornos | Sem valores | Manutenção | Ver valores com Anderson / Oliveira |
| **Movimentação** | **2.500** | Manutenção | Verbalmente com Anderson, pior cenário, via Transexcede |
| **Cofre elétrico (tornos)** | **1.006** | Thiago Queiroz (FlexMaster) | Orçamento enviado por e-mail |

### 15.5 Resumo de investimento por linha

| Item | Linha 10 — Qtd | Linha 10 — Valor (R$) | Linha 40 — Qtd | Linha 40 — Valor (R$) |
|---|---|---|---|---|
| Trilho Viemar roletado (3 m) | 1 | 2.078,97 | 1 | 2.078,97 |
| Trilho Viemar roletado (4 m) | 1 | 2.677,10 | 1 | 2.677,10 |
| Caixa BIN NR3 | 384 | 641,28 | 119 | 198,73 |
| Instalação elétrica | 2 | (não valorado) | 2 | (não valorado) |
| Instalação pneumática | 2 | 7.000,00 | 2 | 7.000,00 |
| Nivelamento | 1 | (não valorado) | 1 | (não valorado) |
| Cofre elétrico (tornos) | 1 | 1.006,00 | 1 | 1.006,00 |
| **Subtotal valorado** | | **13.403,35** | | **12.960,80** |

*(A planilha apresenta `#VALUE!` nos totais por causa dos campos não valorados.)*

### 15.6 Solicitações de Compra e Ordens de Compra efetivadas

| Item | SC | OC | Status | Valor (R$) | Fornecedor |
|---|---|---|---|---|---|
| Caixa BIN NR4 | 448693 | 906363 | APROVADA | 1.668,00 | Ferramentas Gerais Com. e Imp. S.A |
| Tubo e cantoneira | 448623 | 906373 | APROVADA | 2.700,00 | Cofercan Com. de Ferros Canoense Ltda |
| Trilho TR40GP | 448773 | 906773 | APROVADA | 572,53 | — |
| Material elétrico | 448883 | 906333 | APROVADA | 4.338,37 | Real Center Materiais e Equip. Elétricos |
| MO elétrica | 448913 | 906343 | APROVADA | 1.890,00 | Leonir da Silva Manutenção |
| Material pneumático | 448893 | 906463 | APROVADA | 1.062,00 | — (prazo 3 dias) |
| MO pneumática | 448903 | 906353 | APROVADA | 1.150,00 | Pneumax |
| Movimentação | 448863 | 906313 | APROVADA | 2.062,50 | Trans Excede Transportes Excedentes |
| Nivelamento | 448873 | 906323 | APROVADA | 3.707,70 | Oliveira Manutenção e Rep. de Máq. Ind. |
| Cofre | 447203 | 904303 | APROVADA | 1.119,18 | FMC Ind. de Equip. Elétricos |
| Frete | 449593 | — | — | 540,00 | Transexcede (barras e tubo) |
| Caixa BIN NR4 | 450253 | 908793 | APROVADA | — | — |
| | | | **TOTAL C/ IMPOSTOS** | **R$ 20.810,27** | |

> **Observação:** o custo real das OCs (R$ 20.810,27) é **55 % maior** que o estimado para a Linha 10 (R$ 13.403,35), principalmente por: nivelamento (3.707,70 contra 3.000 estimado), material elétrico (4.338,37, que não tinha valor estimado) e frete (540,00, não previsto). **Lição aprendida para os próximos pilotos: incluir elétrica e frete no orçamento base.**

### 15.7 Cronograma de implantação (72 dias — aba `Prazos`)

| Dia início | Duração | Atividade |
|---|---|---|
| 1 | 3 | Validação de layout com lideranças (Marceli, L. Bos) |
| 4 | 3 | Realizar alterações necessárias após validação |
| 8 | 1 | Realizar alterações necessárias após validação |
| 8 | 5 | **Fazer CAPEX** |
| 9 | 4 | Iniciar orçamentação com compras |
| 15 | 5 | **Aprovação CAPEX** |
| 22 | 3 | Fazer SC e aprovação de OC de materiais e serviços |
| 22 | 20 | **Virada de roteiros e recursos/equipamentos no Tecnicon (ERP)** |
| 23 | 4 | Chegada de materiais |
| 29 | 5 | Fabricação de trilhos roletados (1 unidade) — internamente, 1 semana/trilho |
| 34 | 1 | Instalar elétrica e pneumática para 2 equipamentos |
| 36 | 5 | Fabricação de trilhos roletados (unidade 2) |
| 41 | 1 | Instalar elétrica e pneumática para 2 equipamentos |
| 43 | 5 | Fabricação de trilhos roletados (unidade 3) |
| 50 | 5 | Fabricação de trilhos roletados (unidade 4) |
| 52 | 3 | **Treinamento de operadores, logística e PCP** |
| 55 | 2 | **Virada de layout com nivelamento de máquinas** |
| 57 | 5 | Semana de try-out e ajustes |
| 64 | 5 | **Fechamento do piloto / avaliação de resultados e próximos passos** |

**Caminho crítico identificado:** CAPEX (dias 8-20, **13 dias**) → compras (22-27) → fabricação de trilhos (**29-55, 26 dias — 4 trilhos × 1 semana, em série**) → virada (55-57). **A fabricação interna dos trilhos, em série, é 36 % do cronograma total.** Fabricar em paralelo (ou terceirizar 2 unidades) reduziria o projeto em ~15 dias.

**ERP:** a "virada de roteiros e recursos" no **Tecnicon** leva 20 dias e corre em paralelo — é o item de maior risco oculto, pois sem roteiros corretos no ERP o PCP não consegue programar a nova configuração.

### 15.8 Cronograma macro de rollout (arquivo `fluxo macro.xlsx`)

| Atividade | Nov 2023 (S3-S4) | Dez 2023 (S1-S4) | 2024 (Jan-Nov) |
|---|---|---|---|
| Comunicação | ✔ | | |
| Treinamento das equipes | ✔ | | |
| Piloto | | ✔ | |
| Férias coletivas | | ✔ (Dez) | |
| Avaliação dos resultados e próximos passos | | ✔ | |
| **FLUXO TERMINAL DE DIREÇÃO** | | | ✔ (primeiro) |
| FLUXO ARTICULAÇÃO AXIAL | | | ✔ |
| FLUXO PIVÔ DE SUSPENSÃO (QUENTE) | | | ✔ |
| FLUXO PIVÔ DE SUSPENSÃO e PISTÃO | | | ✔ |

> O **Terminal de Direção é a primeira família do rollout**, confirmando seu papel de piloto para toda a transformação de fluxo da fábrica.

---

## 16. SETUP / TROCA RÁPIDA DE FERRAMENTAS (TRF)

### 16.1 Por que isso importa para o TD10

Os setups no TD10 consomem, conforme §8:

| Setup | Tempo (s) | Tempo (min) | % das perdas |
|---|---|---|---|
| Setup Pino | 720 | 12 | 2,6 % |
| Setup Equiptop | 1.758 | 29,3 | 6,2 % |
| Setup Caixa | 1.800 | 30 | 6,4 % |
| **Total** | **4.278** | **71,3** | **15,2 %** |

E no GBO TERMINAL, rateados por peça (base 450 pç/lote):

| Setup | s/peça | % do tempo manual |
|---|---|---|
| Setup Pino (594 s) | 1,320 | 2,2 % |
| Setup Equiptop (1.674 s) | 3,720 | 6,2 % |
| Setup Caixa (1.800 s) | 4,000 | 6,7 % |
| **Total** | **9,04** | **15,1 %** |

> ⚠ **Atenção à premissa de lote:** o rateio é feito sobre **450 peças**. Se o projeto de fluxo por família reduzir o lote (que é justamente o objetivo), **o impacto do setup por peça aumenta proporcionalmente**. Com lote de 225 peças, os 9,04 s/pç viram **18,08 s/pç** — inviabilizando o takt.
>
> **Conclusão estratégica: a TRF é PRÉ-REQUISITO para a redução de lote.** Não é um projeto paralelo, é um projeto habilitador. Sem SMED, reduzir lote degrada a capacidade.

### 16.2 Método Shingo (conforme o deck `Troca Rápida de Ferramentas.pptx`)

**Definições:**
- **SETUP:** ato de trocar e ajustar dispositivos e ferramentas de uma máquina que produz uma peça para produzir outro tipo.
- **TEMPO DE SETUP:** tempo decorrido **desde a última peça boa de um lote até a primeira peça boa do lote seguinte**, incluindo os ajustes após a troca do ferramental.
- **SMED (Single Minute Exchange of Die):** setups em **menos de 10 minutos**.

**Histórico (19 anos de desenvolvimento):**
- **1950** — Análise de gargalos na planta Mazda, Hiroshima → conceitos de setup interno e externo.
- **1957** — Estaleiro Mitsubishi, Hiroshima → importância do setup externo.
- **1969** — Toyota exige reduzir setup de prensas de **4 horas para 3 minutos** → nascimento do SMED.

**As 4 etapas básicas de um setup:**
- **A)** Preparação, ajuste e verificação da matéria-prima (localização de peças/ferramentas, estado de funcionamento, remoção/limpeza/retorno de ferramentas do último item).
- **B)** Montagens e desmontagens de ferramentas (remoção e fixação para o próximo lote).
- **C)** Medições, ajustes e calibrações (centragens, alinhamentos, ajustes finos, temperatura, pressão, vazão).
- **D)** Teste para início da produção e ajustes (alimentação, 1ª peça, processo, tentativa, inspeção, erro, amostra).

**Os 3 passos do método:**

| Passo | Ação | Ganho típico |
|---|---|---|
| **1** | **Separar** a preparação em INTERNA (máquina parada) e EXTERNA (máquina operando) | **~50 % de redução só com isso** |
| **2** | **Transferir** o máximo possível de interna para externa (trocar módulos não partes, pré-aquecimento, ferramentas reservas no gargalo, máquinas reservas em paralelo no gargalo) | Adicional significativo |
| **3** | **Racionalizar** todos os aspectos do setup, internos e externos | Contínuo |
| **Adicional** | **Eliminar ajustes e regulagens** — o ajuste consome de **50 % a 70 % do tempo total de troca interna** | O maior bloco |

**O método de análise em 6 passos:**

| Passo | Conteúdo |
|---|---|
| 1 | Selecionar a máquina, justificar a escolha, formalizar objetivos de redução e ganhos, brainstorming inicial |
| 2 | **Estudo do procedimento existente:** filmagem do setup mais completo, cronoanálise detalhada, curva ABC das atividades, classificação interno/externo |
| 3 | **Conversão interno → externo:** pré-montagens, ajustes externos, melhoria de ferramental, agilização de fixações, eliminação de ajustes; elaborar **roteiro de setup** e plano de ação |
| 4 | Executar as melhorias do plano de ação |
| 5 | Executar o setup conforme o novo procedimento e comparar planejado × realizado |
| 6 | **Padronização:** instruções de trabalho, treinar, elaborar o Manual de Setup |

**Os inimigos da TRF:**
- *"Os **parafusos** são o inimigo número 1 da TRF"* — parafuso = aumento do setup interno.
- *"A **gambiarra** é o inimigo número zero da TRF"* — gambiarra = aumento da variabilidade.

**Tripé da TRF:** **operador** · **máquina** · **ferramental** — os três vértices precisam ser tratados.

**Soluções técnicas catalogadas:** cam lock, porca borboleta, arruelas "C", rasgos com acesso (afrouxar e arrastar), magnetismo, fixadores mais curtos, menos elementos de fixação, engates rápidos hidráulicos, linhas codificadas por cor, código de cores (parafusos/porcas, ferramentas/dispositivos, matrizes), código de números, **PRE-SET** (pré-montagem, pré-corte, pré-ajuste, pré-aquecimento).

**Análise do ajuste (5 perguntas):** Motivo (que função atende?) · Causa (que condições criam a necessidade?) · Método (qual é o atual?) · Alternativas (que melhorias reduzem/eliminam?) · Procedimento (está padronizado?).

### 16.3 Modelo de estratificação de setup (arquivo `Exemplo de estratificação de set up.xlsx`)

Este arquivo é um **modelo metodológico com dados reais de outras máquinas da planta** (extrusoras, PH630-02, CNC20, CNC21). É o template que deve ser aplicado ao TD10.

**Estrutura do modelo:**

| Bloco | Conteúdo |
|---|---|
| Série histórica | Tempo médio, frequência e disponibilidade por mês (2015 a 2021) |
| Meta | Tempo-alvo de setup |
| Pareto por turno | Participação de cada turno no tempo total de setup |
| Mapa de elementos de tempo | Cronoanálise elemento a elemento, com classificação em 6 categorias |
| Plano de ação | O que fazer / Por que fazer / Quem / Quando / Quanto / Ganho (min/mês) / Status |

**Classificação de 6 categorias usada:**

| Sigla | Categoria |
|---|---|
| **T** | Troca |
| **R** | Regulagem |
| **Q** | Qualidade |
| **P** | Procura |
| **O** | Outros |
| **A** | Anomalia |

**Exemplo real — CNC20/CNC21, setup de 29/06/2021 (peça que entra: C626245):**

| Categoria | Tempo |
|---|---|
| Regulagem | 00:19:04 |
| Qualidade | 00:15:29 |
| Troca | 00:12:22 |
| Outros | 00:12:18 |
| Anomalia | 00:02:24 |
| **Procura** | **00:00:52** |

Primeiros elementos cronometrados:

| Classe | Tempo corrido | Tempo por operação | Otimizável | Elemento |
|---|---|---|---|---|
| T | 00:00:46 | 00:00:46 | | Retirar pinça |
| O | 00:01:20 | 00:00:34 | | Limpar pinça e porta-pinça |
| T | 00:01:25 | 00:00:05 | | Colocar a pinça |
| T | 00:03:42 | 00:02:17 | **00:02:17** | Montar contrapeso na tampa do porta-pinça |
| T | 00:04:00 | 00:00:18 | | Montar tampa na máquina |
| **A** | 00:05:30 | 00:01:30 | **00:01:30** | **Desmontar contrapeso no porta-pinça** (retrabalho) |
| **A** | 00:06:24 | 00:00:54 | **00:00:54** | **Montar tampa na máquina** (repetição) |
| R | 00:10:15 | 00:03:51 | **00:03:51** | Aproximar barra na pinça e anotar valor em Z |
| R | 00:10:26 | 00:00:11 | | Afastar torre |
| O | 00:10:36 | 00:00:10 | | Limpar torre |
| T | 00:12:16 | 00:01:40 | | Soltar parafusos do VDI para troca de ferramenta |
| **P** | 00:12:40 | 00:00:24 | **00:00:24** | **Procurar chave Allen** |
| T | 00:13:05 | 00:00:25 | | Soltar parafusos do VDI |
| T | 00:13:20 | 00:00:15 | **00:00:15** | Soltar bucha da ferramenta |
| O | 00:13:37 | 00:00:17 | **00:00:17** | Limpar bucha da ferramenta |
| T | 00:14:42 | 00:01:05 | | Trocar ferramenta da bucha |
| T | 00:16:48 | 00:02:06 | **00:02:06** | Fixar ferramenta do VDI |
| R | 00:21:25 | 00:01:01 | | Zerar corretores das ferramentas antes do Preset |
| R | 00:23:00 | 00:01:35 | | Aproximar broca em Z na pinça e realizar Preset em Z |
| R | 00:24:19 | 00:01:19 | | Aproximar ferramenta em Z na pinça e Preset em Z |
| R | 00:27:10 | 00:02:51 | | Aproximar ferramenta em X na pinça e Preset em X |

**Planos de ação já existentes (aplicáveis ao TD10):**

| Ação | Por que fazer | Responsável | **Ganho (min/mês)** |
|---|---|---|---|
| **Desenvolver lista de dispositivos × forjado** | Não procurar dispositivos durante o setup (8 min) | Qualidade | **344** |
| **Pré-preencher registro de inspeção de conformação e diário de bordo** | Evitar perda de 4 minutos | Produção | **172** |
| **Colocar computador em cada posto de trabalho** | Evitar deslocamento para impressão (2 min) | Roger | **86** |
| **Padronizar programas específicos para cada peça** | Evitar correção ou colisão (1 min); não usar programa de outra peça | Produção | **43** |
| Realizar Preset de dispositivos de medição para cada máquina e peça | Não procurar dispositivos durante o setup | Preset | — |
| Treinamento conforme roteiro de setup | Reduzir variação dos tempos de setup | Produção | — |
| Padronizar molas necessárias para os setups | Evitar molas erradas (faces não paralelas) | Preset | — |
| Preset imprimir o desenho | Evitar deslocamento para impressão (2 min) | Preset | — |
| Avaliar método de medição de micrômetro (passa/não passa) | Reduzir variação | Qualidade | — |
| Criar checklist para setup | Reduzir variação | Qualidade | — |
| Entregar calços nominal, +1 e −1 durante o setup | Reduzir variação | Qualidade | — |
| Preparador ter calços em frente à máquina | Reduzir variação | Produção | — |
| Não desmontar setups dos produtos de maior volume | Reduzir variação | Produção | — |
| Criar chave para soltar porca com mais facilidade | Reduzir variação | Processo | — |
| Pintar/gravar furos para molas centrais | Reduzir variação | Preset | — |
| Revisar estoque mínimo de calços e molas | Reduzir variação | Preset | — |
| Desenvolver luva para manusear peça quente | Evitar acidentes | Segurança | — |
| Melhorar calha de saída para não cair peça na mesa | Evitar acidentes | Manutenção | — |
| Fabricar/adquirir duas tampas (CNC) | Evitar tempo interno | Lucas | — |
| Montar contrapeso na tampa do porta-pinça fora da máquina | Evitar tempo interno | Lucas | — |
| Medir dimensões das ferramentas fora da máquina | Evitar tempo interno | Preset + Processo | — |
| Criar layout de ferramentas para o mix de peças | Evitar tempo interno | Lucas | — |
| Melhorar sistema de zeramento das ferramentas | Implantar preset automático | Processo | — |
| **Criar perfil para medição no projetor de perfil** | **Evitar medição ponto a ponto da cota C** | Processo | — |
| Criar roteiro de setup | Evitar tempo interno | Processo | — |

> **Ganho quantificado já identificado: 645 min/mês = 10,75 h/mês** só nas 4 ações valoradas. Aplicadas ao TD10, isso representa ~**1,3 % de disponibilidade adicional**. E a ação *"Criar perfil para medição no projetor de perfil"* ataca diretamente os **5,0 s/pç da "Inspeção Pino projetor"** identificada no GBO TD10 — **é a 3ª maior atividade do TD10**.

**Dados históricos de setup de outras máquinas (benchmark interno):**

| Máquina | Tempo médio 2021 (min) | Meta (min) | Frequência/mês | Disponibilidade perdida |
|---|---|---|---|---|
| Extrusoras 1/2 | 28,51 | **10** | 127,4 | 6,87 |
| PH630-02 | 40,33 | **28,23** | 44,7 | 5,52 |
| CNC 20 | 46,41 | **32,48** | 40,8 | 5,42 |
| CNC 21 | 54,89 | **38,43** | 36,2 | 5,83 |

**Pareto por turno (CNC20):** 1º turno 7,7 % · 2º turno 43,9 % · 3º turno 48,4 % — **os turnos 2 e 3 concentram 92 % do tempo de setup**, o que é um achado de treinamento/supervisão, não de método.

| Máquina | Tempo médio 1º turno | 2º turno | 3º turno |
|---|---|---|---|
| Extrusoras | 22,0 min | 20,3 min | **28,8 min** |
| PH630-02 | **50,3 min** | 32,4 min | 32,5 min |
| CNC 20 | 18,3 min | **56,8 min** | 36,2 min |
| CNC 21 | 24,0 min | **57,8 min** | 56,7 min |

> **A variação de tempo de setup entre turnos chega a 3,1× (CNC20: 18,3 vs 56,8 min).** Isso **não é um problema de método, é de padronização e treinamento** — e é o ganho mais barato disponível.

---

## 17. ERGONOMIA E ANTROPOMETRIA DOS POSTOS

**Fonte:** `Antropometria_PostosdeTrabalho[1].pdf`

### 17.1 Tabela antropométrica de referência (cm)

| Medida | Critério | Mulheres 5% | Mulheres 95% | Homens 5% | Homens 95% | **Medida adotada** |
|---|---|---|---|---|---|---|
| A. Estatura | MÁX | 151,0 | 172,5 | 162,9 | 184,1 | **184,1** |
| B. Altura da cabeça sentado | MÁX | 80,5 | 91,4 | 84,9 | 96,2 | **96,2** |
| C. Altura dos olhos sentado | MÍN | 68,0 | 78,5 | 73,9 | 84,4 | **68,0** |
| D. Altura dos ombros sentado | MÍN | 53,8 | 63,1 | 56,1 | 65,5 | **53,8** |
| E. Altura do cotovelo sentado | MÁX | 19,1 | 27,8 | 19,3 | 26,0 | **26,0** |
| F. Largura das pernas | MÁX | 11,8 | 17,3 | 11,7 | 15,7 | **17,3** |
| G. Altura do assento (poplítea) | MÁX | 35,1 | 43,4 | 39,9 | 48,0 | **48,0** |
| H. Profundidade do tórax | MÁX | 23,8 | 35,7 | 23,3 | 31,8 | **35,7** |
| I. Comprimento do antebraço | MÍN | 29,2 | 36,4 | 32,7 | 38,9 | **29,2** |
| J. Comprimento do braço | MÍN | 61,6 | 76,2 | 66,2 | 78,7 | **61,6** |

**Lógica de projeto aplicada:** medidas de **alcance** usam o **percentil 5 % feminino** (garante que a pessoa menor alcance) e medidas de **espaço/folga** usam o **percentil 95 % masculino** (garante que a pessoa maior caiba). É a prática correta.

### 17.2 Critérios de posto

**Posto de trabalho — posição SENTADA:**

| # | Critério |
|---|---|
| 1 | Altura da superfície de trabalho para atividade |
| 2 | **Espaçamento (E) para acomodar os membros inferiores**: E ≥ 70 cm = **BOM** · E entre 50 e 70 cm = **ACEITÁVEL** · E ≤ 50 cm = **SOFRÍVEL** |
| 3 | Altura ótima do assento |
| 4 | Superfície para apoio dos antebraços com os braços soltos |

**Posto de trabalho — posição EM PÉ:**

| # | Critério |
|---|---|
| 1 | Altura da superfície de trabalho |
| 2 | Superfície para os braços soltos |
| 3 | Superfície para apoio dos antebraços |
| 4 | Superfície para agarrar peças pesadas |

### 17.3 Aplicação ao TD10

**Riscos ergonômicos identificados nos demais documentos:**

| Risco | Evidência | Documento |
|---|---|---|
| **Fadiga elevada no posto MASTER** | Coeficiente de fadiga **13,04 %** contra 4,76 % dos demais postos; **22 movimentações** por ciclo | Yamazumi |
| **Manuseio de carga** | Caixas de 15 kg; peso máximo projetado de 45 kg/m linear no trilho | Projeto fluxo por família |
| **Transporte manual de caixas acumuladas** | "Levar as caixas fechadas acumuladas para colocar no palete" — 120 s a cada 90 pç | Yamazumi |
| **Atividade de "bater caixas"** | 2 ocorrências no GBO TERMINAL (trilho gargalo e trilho de saída), 180 s cada | GBO TERMINAL |
| **Peça quente** | Ação de plano: "Desenvolver luva para manusear peça quente — evitar acidentes" | Estratificação de setup |
| **Deslocamentos** | 10 s/peça de deslocamento (maior item do GBO) | GBO TERMINAL |

**Conformidade das alturas projetadas nos trilhos:**

| Elemento | Altura projetada | Avaliação ergonômica |
|---|---|---|
| Entrada do trilho (com rodízio) | **0,885 m** | ✅ Adequado para trabalho em pé (faixa 0,85–0,95 m para trabalho leve/preciso) |
| Saída do trilho (com rodízio) | **0,785 m** | ✅ Adequado para trabalho em pé com força (faixa 0,75–0,85 m) |
| Entrada sem rodízio | 0,720 m | ⚠ Baixo — exige flexão de tronco |
| Saída sem rodízio | 0,650 m | ❌ Muito baixo — risco lombar |

> **Recomendação:** os trilhos **devem** ser instalados com rodízios (configuração já orçada), pois a versão sem rodízio fica abaixo da faixa ergonômica aceitável.

**Nota do deck de TRF sobre segurança:**
> *"Após reorganizar a célula, o time precisa revisar todos os processos e identificar se existem atividades consideradas como risco de segurança. Uma avaliação de risco deve ser conduzida na atividade considerada com risco de segurança, levantando os resultados e ações propostas validadas pelo Gerente de Linha ou responsável pela segurança."*

**→ Ação obrigatória: avaliação de risco ergonômico formal na virada de layout do TD10.**

---

## 18. REFERENCIAL DE PPCP (WORKSHOP DE SINCRONIZAÇÃO)

**Fonte:** `workshop_pps_v1.pdf` — Carlos E. P. Panitz, MSc. — 05/02/2018 — 120 slides, elaborado para a **Viemar**.

Este material é o **referencial conceitual** que sustenta o projeto de fluxo por família. Os pontos aplicáveis ao TD10:

### 18.1 Estratégia de atendimento

| Estratégia | Característica | Ponto de desacoplamento |
|---|---|---|
| **MTS** (Make-To-Stock) | Circuito aberto · acionado por previsão | Estoque de produto acabado |
| **MTO** (Make-To-Order) | Circuito fechado · acionado por ordens | Estoque de matéria-prima |
| **ATO** (Assembly-To-Order) | Mistura: componentes genéricos em MTS, variações finais em MTO | Estoque intermediário |

**Blue print definido para a Viemar (slide 50):** **dois circuitos**
1. **Circuito 1 — Usinagem → Montagem** (puxado, por ordens)
2. **Circuito 2 — Corte / Conformação / Tratamento Térmico** (empurrado, por Min/Máx calculado pelo PPCP, onde a demanda é o consumo do mercado), governado por **Heijunka/Kanban**

> **Posicionamento do TD10:** o TD10 está no **Circuito 1**, portanto **deveria operar puxado**. O que o MFV e o Fluxograma Linha 10 mostram, porém, é um sistema **empurrado por ordens centralizadas** ("Esperando OP", "Aguardando OP", "leitura das ordens de produção" na laminação). **Há uma lacuna entre o blueprint projetado e a prática atual.**

**Caso #1 citado (MTO → ATO, postergação):** 7 % das peças básicas / 49 % dos part numbers finais; investimento R$ 300 mil; **redução de inventário R$ 1.800 mil**; payback 1,3 anos (WACC 13 %); CV cai de 198 % (part number) para 98 % (peça genérica).

### 18.2 Política de inventário — modelos de categorização

| Modelo | Base | Foco |
|---|---|---|
| **ABC** | Valor do item | Otimização de estoques |
| **XYZ** | Variabilidade de demanda (CV) | Otimização de estoque e nível de serviço |
| **PQR** | Frequência de consumo/consulta | Otimizar operação, identificar demanda reprimida |

**Matriz de dimensionamento:**

| Categoria | CV | Perfil | Método de ressuprimento |
|---|---|---|---|
| **X — Runner** | CV < 70 % | Alto giro, previsível | **JIS / JIT** |
| **Y — Repeater** | 70 % < CV < 170 % | Médio | **MRP · Kanban / VMI** |
| **Z — Stranger** | CV > 170 % | Esporádico | **MRP · sob consulta** |

**Nível de serviço recomendado:**

| | X | Y | Z |
|---|---|---|---|
| **A** | 99 % | 96 % | 90 % |
| **B** | 96 % | 90 % | 85 % |
| **C** | 90 % | 85 % | 80 % |

**Fotografia de 2017 da Viemar (diagnóstico do workshop):**
- 50 % dos SKUs representam **7 % do faturamento** dos últimos 12 meses.
- Quase 50 % dos SKUs têm perfil de **alta variabilidade (CV acima de 150 %)**.
- Matriz XYZ × ABC: **1.613 SKUs** → X: 731 (45,3 %) · Y: 251 (15,6 %) · Z: 631 (39,1 %); A: 215 (13,3 %) · B: 280 (17,4 %) · C: 1.118 (69,3 %).
- **53 % dos SKUs representam 2,06 % dos pedidos de venda e 34,97 % do estoque** (posição 30/06/2017).
- **70 % do backlog está relacionado a erro/falta de forecast (MAPE > 30 %).**

### 18.3 Por que o MRP/MPS falha (slide 45) — diagnóstico aplicável ao TD10

| Causa | Evidência no TD10 |
|---|---|
| Não se estabelece período firme (roda MRP todo dia) | — |
| MRP executado com capacidade infinita | Perdas de disponibilidade a 106,7 % não aparecem no MRP |
| Produção não segue a programação do PCP | "A peça atende o requisito de priorização linha 10?" no fluxograma |
| **Nasce um PCP "informal" (verbal)** baseado em listas críticas e objetivos locais (otimização de setup, disponibilidade de peça, peças mais simples de fazer) | **"Para onde vão as outras 1.200 pcs???"** no MFV |
| Pessoas se acostumam e esquecem as premissas mínimas | Eficiência de 69,2 % aceita como normal |

### 18.4 Kanban — fórmula de cálculo aplicável

**Tempo de ressuprimento (TR) = T1 + T2 + T3 + T4 + T5 + T6 + Ts**

| Componente | Descrição |
|---|---|
| T1 | Tempo do kanban na caixa aguardando ser recolhido |
| T2 | Tempo de transporte do kanban entre ponto de consumo e produção |
| T3 | Tempo do kanban na fila de espera do quadro de planejamento |
| T4 | Tempo de processamento de um contentor (incluindo setup) |
| T5 | Tempo de espera de transporte de um contentor entre produção e consumo |
| T6 | Tempo de transporte de um contentor entre produção e consumo |
| Ts | Tempo de segurança |

**Exemplo prático do workshop:** T1 = 2 h · T2 = 0,2 h · T3 = 4 h · T4 = 2,5 h · T5 = 1 h · T6 = 0,3 h · Ts = 8 h → **TR = 18 h**. Múltiplo: 36 conj/carrinho · Demanda: 24 conj/h → **Nº de cartões = (24 ÷ 36) × 18 = 9 cartões**, com sinalização verde/amarelo/vermelho.

> **Aplicação ao TD10:** o **space buffer de 9 KLT (162 pç)** definido no projeto de fluxo por família é **exatamente um dimensionamento de kanban**. O que falta é formalizar os cartões e a regra de acionamento.

### 18.5 Estoque de segurança

**Quando se trabalha com previsão:** S = √[Σ(D−F)² / (n−2)]
**Quando se trabalha com consumo:** S = √[Σ(D−D̄)² / (n−1)]
**E_seg = k × S × √(LT/PP)**

Onde k = fator de segurança do nível de serviço (Excel: `INV.NORMP.N(95%)`), LT = lead time médio total, PP = período incremental de avaliação da variabilidade.

**Para CV > 150 % e incidência < 40 %, usar distribuição de Poisson** (dica prática: usar normal como aproximação com σ² = m).

**Para proteção da variabilidade do lead time:** E_seg = k × σ_LT × D̄

### 18.6 As 7 perdas clássicas (Shingo) — mapeadas no TD10

| # | Perda | Evidência no TD10 | Magnitude |
|---|---|---|---|
| 1 | **Superprodução** ("a pior das sete") | WIP oscilante de até 206 pç; buffers de 6.912 pç dimensionados | Alta |
| 2 | **Transporte** | 870 m de movimentação; 10 s/pç de deslocamento | Alta |
| 3 | **Processamento em si** | Medição ponto a ponto da cota C; inspeção em projetor (300 s) | Média |
| 4 | **Produtos defeituosos** | 376 sucatas e 9.425 peças com retrabalho/desvio em 12 meses | Alta |
| 5 | **Espera** | **221 h de espera por processamento (66 % do lead time)** | **Crítica** |
| 6 | **Estoques** | **97 h de espera de lote (29 % do lead time)**; lotes de 1.000-2.200 pç | **Crítica** |
| 7 | **Movimento** | 22 movimentações no posto MASTER; fadiga de 13 % | Média |

> *"A maior de todas as perdas é a perda que não enxergamos."* — Shigeo Shingo

### 18.7 Sinais de logística não-enxuta (checklist aplicado ao TD10)

| Sinal (evidente) | Presente no TD10? | Evidência |
|---|---|---|
| Manuseios intermediários, transbordos, reembalamentos | ✅ SIM | Estoque do recebimento → intermediário → conformação → forjado |
| Pulmões intermediários entre operações | ✅ SIM | WIP antes de Equiptop/Caixa/Montagem/Embalagem |
| Zig-zag | ✅ SIM | 870 m de movimentação; entrada ideal perpendicular ao fluxo proposto (premissa 5) |
| Muitas empilhadeiras | ✅ SIM | Empilhadeira, paleteira e ponte rolante no MFV |
| Muitas ocorrências de ruptura de estoque | ⚠ Provável | Déficit de 332 pç/dia contra demanda |
| Baixa acuracidade de estoque | ✅ SIM | *"Para onde vão as outras 1.200 pcs???"* |

| Sinal (velado) | Presente no TD10? | Evidência |
|---|---|---|
| Inexistência de método de acionamento (apenas experiência e comunicação verbal) | ⚠ Parcial | "A peça atende o requisito de priorização?" |
| Inexistência de trabalho padronizado | ❌ NÃO | TPO040-043 existem e são bons |
| Inexistência de KPIs | ❌ NÃO | Eficiência, IROG, GBO medidos |
| Excesso de transações no ERP | ⚠ Possível | Virada de roteiros no Tecnicon leva 20 dias |
| Estratégia de produção inadequada | ✅ SIM | Circuito 1 deveria ser puxado, opera empurrado |
| Baixa aderência entre datas planejadas e realizadas | ✅ SIM | Tema central dos ganhos "Aderência ao MPS" |
| Decisões de priorização tomadas verbalmente no chão de fábrica | ✅ SIM | Fluxograma Linha 10 |

### 18.8 Heijunka — nivelamento

**Exemplo do workshop (takt 5 min):** modelos A (56), B (29), C (29), total 114.
- **Sequenciamento em lote:** A exige 2 turnos, B exige 2 turnos, C exige 2 turnos → ociosidade, mão de obra dimensionada pelo item de maior tempo de ciclo.
- **Nivelamento por mix:** A a cada 10 min, B a cada 20 min, C a cada 20 min → sequência **ABACABACABACABAC** → **1 turno cada**, mão de obra dimensionada pela **média ponderada**.
- **Benefícios:** mais eficiência na distribuição das atividades · menor exigência da máquina · menor exigência de inventário · mínima mão de obra e inventário, **com maior frequência de setup**.

> **Aplicação direta ao TD10:** as **"viradas" de 3.600 s × 2 = 7.200 s/turno (25,6 % das perdas)** são exatamente o custo do **não-nivelamento**. Ou se nivela o mix (exigindo TRF para suportar mais setups), ou se aceita o lote grande (exigindo lead time de 14 dias). **Não há terceira opção.**

### 18.9 Três dicas de ouro do workshop

1. **Enxergue o fluxo como um sistema e não pelos seus elementos isolados** (é óbvio mas precisa ser exercitado).
2. **Não siga uma única igreja** — para cada tipo de problema existem ferramentas, métodos e abordagens distintos.
3. **Pense no fluxo de materiais desde a concepção de um projeto de produto ou processo.** Nada compensará uma decisão estruturante mal tomada.

### 18.10 O que define um bom fluxo/layout de materiais

- Menor distância percorrida
- "Menor área" física (sem esquecer o sistema — existem trade-offs)
- Menos rupturas de estoques
- Maior produtividade (ex.: linhas separadas por pessoa)
- Menos ocorrências de erros de separação

---

## 19. DIAGNÓSTICO CONSOLIDADO — AS 10 PERDAS ESTRUTURAIS DO TD10

| # | Perda | Magnitude quantificada | Fonte | Severidade |
|---|---|---|---|---|
| **1** | **Paradas planejadas excedem o tempo disponível** | **28.178 s de perdas contra 26.400 s de turno = 106,7 %** | GBO Rev06/07 | 🔴 CRÍTICA |
| **2** | **Lead time 14 dias para 7 h de processamento** | **334,1 h · 2,13 % de VA · 98 % espera** | MFV + Shingo | 🔴 CRÍTICA |
| **3** | **79 % do trabalho manual não agrega valor** | 59,76 s/pç: 21,2 % AV · 46,7 % NNAV · 32,1 % D | GBO TERMINAL | 🔴 CRÍTICA |
| **4** | **Inspeções consomem 47,3 % das paradas** | 13.340 s/turno; inspeção de montagem sozinha = 7.000 s | GBO Rev06/07 | 🔴 CRÍTICA |
| **5** | **Desbalanceamento extremo entre postos** | Op. Montagem a 137 % enquanto 4 operadores a 22-29 % | GBO estado atual | 🟠 ALTA |
| **6** | **Gargalo (pino) opera abaixo da demanda** | 2.856 pç/dia nominal × 69,2 % = 1.976 pç/dia vs 2.308 pç/dia demandadas (**−14 %**) | GBO + demanda | 🟠 ALTA |
| **7** | **Viradas consomem 25,6 % das paradas** | 7.200 s/turno (ou 10.800 s na aba Planilha2) | GBO Rev06/07 | 🟠 ALTA |
| **8** | **Setups longos e com variação de 3,1× entre turnos** | 4.278 s/turno; CNC20: 18,3 min (1ºT) vs 56,8 min (2ºT) | GBO + estratificação | 🟠 ALTA |
| **9** | **Sucata e retrabalho com impacto de faturamento** | 376 sucatas + 9.425 pç com retrabalho/desvio (12 meses) = **R$ 103.488 de faturamento afetado** | Projeto capabilidade | 🟡 MÉDIA |
| **10** | **Perda de rastreabilidade de WIP** | *"Para onde vão as outras 1.200 pcs???"*; 870 m de movimentação | MFV | 🟡 MÉDIA |

### 19.1 Relação causa-efeito

```
                     LOTES GRANDES (1.000 – 2.200 pç)
                              │
              ┌───────────────┼───────────────┐
              ▼               ▼               ▼
      Espera de lote    Setups longos    WIP alto
        (97,3 h)        (justificam     (6.912 pç)
              │          o lote grande)      │
              │               │              │
              └───────────────┼──────────────┘
                              ▼
                  LEAD TIME DE 14 DIAS
                              │
                              ▼
          Baixa aderência ao MPS · Atrasos · Backlog
                              │
                              ▼
         "Listas críticas" · Priorização verbal · PCP informal
                              │
                              ▼
      Mais viradas emergenciais · Mais setups não planejados
                              │
                              └──────► (realimenta o ciclo)
```

```
    INSPEÇÃO MANUAL EM PAPEL (FO021)
              │
    ┌─────────┼──────────┐
    ▼         ▼          ▼
13.340 s   Erros de   24 h de parada
de parada  transcrição  por estudo de
por turno              capabilidade
    │         │          │
    └─────────┼──────────┘
              ▼
    PERDAS = 106,7 % DO TURNO
              ▼
      EFICIÊNCIA DE 69,2 %
              ▼
   CAPACIDADE EFETIVA 1.976 pç/dia
              ▼
    DÉFICIT DE 332 pç/dia (−14 %)
```

### 19.2 Os 3 pontos de alavancagem

| Alavanca | Ataca | Impacto estimado | Projeto |
|---|---|---|---|
| **1. Eliminar inspeção manual no gargalo** | Perdas #1, #4, #9 | **−59 % das perdas de disponibilidade** · eficiência 69,2 % → ~85 % | **MeasurLink (Fase 1)** |
| **2. Reduzir lote e implantar puxada física** | Perdas #2, #7, #10 | **Lead time 14 d → ~6 d (−56 %)** | **Fluxo por família** |
| **3. Rebalancear a célula** | Perdas #3, #5 | **5 → 3 operadores (−40 % MOD)** | **GBO cenário 1** |

**Sequência obrigatória:** **TRF → MeasurLink → Redução de lote → Rebalanceamento.**
Razão: reduzir lote sem TRF degrada a capacidade (§16.1); rebalancear sem MeasurLink é impossível (as inspeções sozinhas são 18,65 s/pç contra takt de 28-30 s).

---

## 20. PLANO DE AÇÃO RECOMENDADO

### FASE 0 — Consolidação dos dados (0 a 30 dias) · Custo: ~0

| Ação | Responsável sugerido | Entregável |
|---|---|---|
| Resolver divergências de dados (§21): capacidade do gargalo (113 vs 119 vs 128 pç/h), virada (7.200 vs 10.800 s), tempo de inserir bucha (2 vs 8,22 s) | Engenharia de Processos | **GBO TD10 Rev08 — versão única e oficial** |
| Eliminar duplicatas e arquivos temporários do repositório; instituir controle de revisão | Engenharia | Repositório limpo com convenção de nomes |
| Medir **IROG real do pino** por 30 dias (disponibilidade × performance × qualidade) | Produção | Baseline auditado do gargalo |
| Confirmar demanda atual (62.332 pç/mês é de qual período?) | PCP | Takt time atualizado |

### FASE 1 — TRF nos 3 setups do TD10 (30 a 90 dias) · Custo: baixo (interno)

| Ação | Base metodológica | Ganho esperado |
|---|---|---|
| Filmar os 3 setups (pino 720 s, Equiptop 1.758 s, caixa 1.800 s) no setup mais completo | Passo 2 do Método Shingo | Diagnóstico |
| Classificar elementos em T/R/Q/P/O/A usando o template de estratificação | `Exemplo de estratificação de set up.xlsx` | Pareto por categoria |
| Separar interno/externo e converter | Passos 1 e 2 | **~50 % de redução só com a separação** |
| Aplicar as 25 ações do plano já catalogado (lista de dispositivos, pré-preenchimento de registros, computador no posto, padronização de programas) | Estratificação de setup | **645 min/mês já quantificados** |
| Criar **roteiro de setup** e Manual de Setup; treinar os 3 turnos | Passo 6 | Eliminar a variação de 3,1× entre turnos |
| **Meta: reduzir setups de 71,3 min para ≤ 36 min (−50 %)** | | **−2.139 s/turno (−7,6 % das perdas)** |

### FASE 2 — MeasurLink Fase 1 no gargalo (30 a 105 dias) · Custo: R$ 56.419,16

| Ação | Prazo | Ganho |
|---|---|---|
| Executar o **piloto gratuito de 45 dias** da Mitutoyo (sem custo) | Imediato | Validação de conceito |
| Liberar CAPEX de R$ 56.419,16 | — | — |
| Implantar na **máquina gargalo (pino)** | **15 dias** após CAPEX | **Inspeção pino: 1.020 s + 300 s/pç no projetor** |
| Criar perfil de medição no projetor (ação já catalogada) | Paralelo | **Elimina medição ponto a ponto da cota C** |
| Digitalizar o diário de bordo e o quadro (3.360 s/turno) | Paralelo | **−11,9 % das perdas** |
| Implantar alerta e bloqueio de máquina por fora de tolerância | Fase 1 | Base do "Defeito Zero" |
| Expandir para a linha TD10 completa | **90 dias** após CAPEX | **Inspeções: −47,3 % das perdas** |
| **Meta combinada Fases 1+2: perdas de 28.178 s → ~17.500 s (razão de 106,7 % → 66,3 %)** | | **Eficiência 69,2 % → ~85 %** |

**Retorno:** R$ 107.770 em ganhos pontuais + R$ 161.832 em riscos evitados contra R$ 56.419,16 → **ROI de 91 % apenas com ganhos pontuais**.

### FASE 3 — Fluxo por família (60 a 130 dias) · Custo: R$ 20.810,27 (já aprovado)

| Ação | Referência |
|---|---|
| Executar o cronograma de 72 dias já elaborado | `Projeto fluxo por familia`, aba Prazos |
| **Paralelizar ou terceirizar 2 dos 4 trilhos roletados** (hoje em série, 26 dias) | Reduz o projeto em ~15 dias |
| Instalar trilhos **com rodízio** (alturas 0,885 m entrada / 0,785 m saída) | §17 — conformidade ergonômica |
| Implantar lote de **450 peças** | Premissa 6 |
| Implantar **space buffer de 9 KLT (162 pç)** com regra formal de kanban (verde/amarelo/vermelho) | §18.4 |
| Implantar as **regras de WIP cap** do fluxograma do teste piloto ("trilho cheio → interromper") | `Fluxograma do Teste Piloto` |
| **Virada de roteiros no Tecnicon (20 dias) — iniciar imediatamente, é o risco oculto do cronograma** | Aba Prazos |
| Treinar operadores, logística **e PCP** (3 dias) | Aba Prazos |
| **Meta: lead time 334 h → ≤ 150 h (−55 %)** | |

### FASE 4 — Rebalanceamento da célula (130 a 160 dias) · Custo: ~0

| Ação | Referência |
|---|---|
| Após MeasurLink, **recalcular o GBO sem o tempo de inspeção manual** | §5, §7 |
| Implantar o **CENÁRIO 1 de 3 operadores** (Op1 15,17 s · Op2 23,86 s · Op3 20,00 s, takt 28 s) | §7.4 |
| Validar que as atividades de controle remanescentes cabem na folga de 14,8 % do posto crítico | §7.4 |
| **Montagem:** rebalancear os 10 postos ao redor do gargalo de 12,98 s ("Colocação de Abraçadeira 2") | §9.1 |
| **Montagem:** padronizar a "Colocação de Abraçadeira (2)" — variação de 163 % (7,5 a 19,75 s) | §9.1 |
| **Montagem:** replicar o buffer da marcação a laser nos demais postos (**redução comprovada de 31 %**) | §9.1 |
| **Yamazumi:** corrigir o cenário proposto — transferir ~2,5 s do OP4 (10,16 s) para o OP3 (3,76 s) | §9.2.3 ⚠ |
| **Pressmatik:** padronizar o elemento "Caixinha" (12,22 s, variação de 7,72 a 15,80 s) para fechar o gap de 2,76 s contra o takt | §10.5 |
| **Laminadoras:** consolidar em 2 operadores **somente após TRF** (hoje a 91-93 % de ocupação) | §11.4 |
| **Meta: 5 → 3 operadores na célula (−40 % MOD) e montagem de 10 → 6 postos** | |

### FASE 5 — Sustentação e rollout (160+ dias)

| Ação |
|---|
| Auditoria periódica do trabalho padrão (TPO040-043) — **revisar TPO043 para remover o check com pincel atômico** |
| Revisar PC001, PC033 e NPU0013 à luz do MeasurLink |
| Avaliação de risco ergonômico formal da nova célula (obrigatório na virada de layout) |
| Replicar o modelo para **TD20, TD30, TD40** (Projeto F4 — R$ 124.257,48 restantes na família Terminal) |
| Seguir o cronograma macro: Terminal → Axial → Pivô Quente → Pivô e Pistão |
| Implantar heijunka/nivelamento de mix para eliminar as viradas |

### 20.1 Resumo financeiro do plano

| Fase | Investimento (R$) | Retorno quantificado (R$) | Prazo |
|---|---|---|---|
| Fase 0 — Consolidação | ~0 | (habilitador) | 30 d |
| Fase 1 — TRF | ~0 (interno) | 645 min/mês + 2.139 s/turno de disponibilidade | 90 d |
| **Fase 2 — MeasurLink** | **56.419,16** | **107.770 pontual + 161.832 risco evitado + 681,72/mês** | 105 d |
| **Fase 3 — Fluxo por família** | **20.810,27** (aprovado) | Lead time −55 % → redução de capital de giro | 130 d |
| Fase 4 — Rebalanceamento | ~0 | **2 operadores/turno × 3 turnos = 6 postos** | 160 d |
| **TOTAL TD10** | **R$ 77.229,43** | **> R$ 270.000 + redução de MOD + redução de WIP** | ~6 meses |

---

## 21. LACUNAS, INCONSISTÊNCIAS E CUIDADOS COM OS DADOS

### 21.1 Divergências numéricas encontradas

| # | Item | Valores conflitantes | Fontes | Impacto |
|---|---|---|---|---|
| 1 | **Capacidade do gargalo** | **113 pç/h** (a 75 % IROG) · **119 pç/h** (nominal) · **128 pç/h** | Projeto fluxo / GBO Rev07 / Capabilidade | Afeta todo o dimensionamento |
| 2 | **Tempo de virada** | **3.600 s × 2 = 7.200 s** · **10.800 s** | Aba `PERDAS DE DISPONIBILIDADE` · Aba `Planilha2` | 3.600 s de diferença (13 % das perdas) |
| 3 | **Inserir bucha** | **2,00 s** (cenários) · **8,22 s** (estado atual e Pressmatik) | GBO cenários · GBO estado atual | 6,22 s/pç = 22 % do takt |
| 4 | **Abastecimento Equiptop** | **6,67 s** · **10 s** · **12 s** | Estado atual · Cenários 1-3 · Métodos 1-2 | 80 % de variação |
| 5 | **Abastecimento usinagem caixa** | **5,5 s** · **7 s** · **11 s** · **14 s** | Método 1 · Estado atual · Método 2 · Cenários | 155 % de variação |
| 6 | **Takt time** | **28 s** (cenários) · **30 s** (estado atual/balanceado) · **31,5 s** (Pressmatik) · **37,43 s** (GBO TERMINAL) · **8,22 s** (Yamazumi) | 5 documentos | **Escopos diferentes, mas não documentados** |
| 7 | **Tempo de setup** | Pino: **594 s** (GBO TERMINAL) vs **720 s** (perdas) vs **1.800 s** (Planilha2); Equiptop: **1.674** vs **1.758 s**; Caixa: **1.800 s** (ambos) | 3 abas | Até 203 % de diferença no pino |
| 8 | **Demanda** | **62.332 pç/mês** (TD10) vs **230.000 pç/mês** (montagem MTD) vs **8.500 pç/dia** (laminadoras) | GBO TERMINAL · Yamazumi · Laminadoras | Escopos diferentes (linha vs família vs operação) |
| 9 | **Lead time** | **13,92 dias** (MFV) vs **14,13 dias** (Shingo) | MFV · SHINGO | Diferença de 1,5 % — aceitável |
| 10 | **Tempo de montagem** | **14,86 s** (Rev07 Planilha3-2) · **12,86 s** (Montagem 1) · **13,00 s** (Montagem 2) · **65,19 s** (GBO Montagem, 10 postos) | Múltiplas | Unidade de medida diferente (por posto vs linha) |

### 21.2 Problemas estruturais dos arquivos

| Problema | Arquivo(s) | Recomendação |
|---|---|---|
| **Duplicata byte-idêntica** (MD5 `0303913a41a2...`) | `!!Cópia de Cópia de GBO - TD10 - Rev07.xlsx` e `Cópia de Cópia de GBO - TD10 - Rev07.xlsx` | Excluir uma |
| **Nomes indicando ausência de versionamento** | "Cópia de Cópia de...", prefixo "!!" | Adotar convenção `GBO_TD10_RevXX_AAAA-MM-DD` |
| **Arquivo temporário de lock do Excel** | `Pressmatik/~$Tempos Pressmatik.xlsx` | Excluir |
| **Arquivo de sistema Windows** | `Pressmatik/Thumbs.db` | Excluir e adicionar ao `.gitignore` |
| **Fórmulas com erro `#VALUE!`** | `Projeto fluxo por familia`, aba Valores (linhas 66-72) | Completar valores de elétrica e nivelamento |
| **Fórmulas com erro `#DIV/0!`** | `Exemplo de estratificação de set up`, Pareto CNC20/CNC21 | Corrigir divisores |
| **Datas serializadas como 1900-01-01** | Simulações horárias das Rev06/Rev07 | Formatar como hora, não data-hora |
| **Abas sem nomenclatura significativa** | `Planilha1`, `Planilha2`, `Planilha3 (2)`, `Planilha3 (3)`, `Planilha4` | Renomear |
| **Macros não documentadas** | `Ferramenta GBO + YAMAZUMI.xlsm` | Documentar ou converter para .xlsx |

### 21.3 Documentos citados mas ausentes do repositório

| Documento | Função | Criticidade |
|---|---|---|
| **PC001** | Plano de controle — inspeção do pino | 🔴 Alta — é o gargalo |
| **PC033** | Plano de controle — inspeção do Equiptop (65 s de ciclo) | 🔴 Alta |
| **NPU0013** | Norma de troca de inserto/broca/macho do Equiptop | 🟠 Média |
| **IT 215** | Instrução — abertura de ordem de produção | 🟡 Baixa |
| **IT 147** | Instrução — impressão de etiquetas | 🟡 Baixa |
| **FO021** | Formulário de registro de inspeção (a ser eliminado) | 🟠 Média — é o objeto do MeasurLink |
| **Layout físico da célula** | Desenho do arranjo atual e proposto | 🔴 Alta — mencionado em todos os projetos |
| **Dados de IROG real do gargalo** | Série temporal de disponibilidade/performance/qualidade | 🔴 Alta |
| **Resultado do teste piloto de julho** | Lote de 900 peças, citado na premissa 6 | 🟠 Média |
| **CAPEX aprovado do MeasurLink** | Status da liberação | 🔴 Alta — destrava a Fase 1 |

### 21.4 Datas e validade dos dados

| Documento | Data | Idade (em 10/2025) | Observação |
|---|---|---|---|
| `workshop_pps_v1.pdf` | 05/02/2018 | 7,7 anos | Metodológico — não expira |
| `lista de materiais` / orçamentos | 24/09/2022 | 3,0 anos | ⚠ **Preços desatualizados** |
| `Exemplo de estratificação de set up` | 29/06/2021 | 4,3 anos | Dados de outras máquinas |
| `TPO043` Rev. 0 | 13/11/2023 | 1,9 anos | Vigente |
| `fluxo macro` (cronograma) | Nov/Dez 2023 + 2024 | 1,8-2,8 anos | ⚠ **Cronograma vencido** |
| `TPO043` Rev. 1 | 01/04/2024 | 1,5 anos | Vigente |
| `Projeto de Capabilidade` | 06/08/2024 | 1,2 anos | ⚠ **Verificar se o CAPEX foi liberado** |
| `Ferramenta GBO + YAMAZUMI` | 03/03/2025 | 7 meses | **Mais recente — dado mais confiável** |
| `GBO TERMINAL` (eficiência) | Março/Abril (ano não informado) | ? | ⚠ **Ano não documentado** |

> **Alerta geral:** boa parte dos documentos tem 1 a 3 anos. **Antes de executar qualquer ação do plano, é obrigatório revalidar: demanda atual, eficiência atual, preços de materiais e status dos CAPEX.**

### 21.5 Limitações metodológicas identificadas

1. **Amostras pequenas em cronoanálises:** Pressmatik Cenário 3 e 5 com apenas 6 ciclos; GBO Montagem "Ensacar" com 6 medições; Caixa grande com 3 medições. **Mínimo recomendado: 10 ciclos.**
2. **Coeficiente de fadiga uniforme:** o Yamazumi aplica 4,76 % para quase todos os postos (exceto MASTER, 13,04 %) — valor que parece arbitrado, não calculado por tabela de fadiga reconhecida (ex.: ILO).
3. **Ritmo não avaliado:** a coluna "Ritmo" do Yamazumi está uniformemente em 1,00 — **não houve avaliação de ritmo/esforço do operador**, o que invalida o tempo como "tempo padrão" formal.
4. **Rateio de setup por lote fixo:** todo o GBO TERMINAL rateia setups sobre 450 peças. **Se o lote real variar, todos os tempos/peça mudam.**
5. **Cenários de 3 operadores não incluem atividades de controle** (18,65 s/pç) — **são inexequíveis antes do MeasurLink.**
6. **Cenário proposto do Yamazumi tem gargalo acima do takt** (10,16 s vs 8,22 s) — a proposta de 4 postos, como está, **não é executável** (§9.2.3).
7. **O MFV é Rev. 00** — é um primeiro mapeamento, sem estado futuro desenhado.

---

## 22. GLOSSÁRIO

| Termo | Definição |
|---|---|
| **TD10** | Linha/célula 10 da família Terminal de Direção |
| **GBO** | Gráfico de Balanceamento de Operadores — ferramenta de distribuição de carga entre postos |
| **Yamazumi** | Gráfico de barras empilhadas que mostra a carga de cada operador contra o takt time |
| **MFV / VSM** | Mapa de Fluxo de Valor (Value Stream Mapping) — Rother & Shook, 1998 |
| **Takt time** | Ritmo da demanda = tempo disponível ÷ demanda do período |
| **Tempo de ciclo** | Tempo efetivo entre a saída de duas peças consecutivas |
| **Lead time** | Tempo total da matéria-prima até o produto acabado |
| **Gargalo** | Recurso com menor capacidade, que define a capacidade do sistema |
| **WIP** | Work In Process — material em processo entre operações |
| **IROG** | Índice de Rendimento Operacional Global (equivalente ao OEE) |
| **AV** | Agrega Valor — atividade pela qual o cliente paga |
| **NNAV** | Necessário mas Não Agrega Valor — ex.: setup, inspeção |
| **D / NAV** | Desperdício — atividade a eliminar |
| **TAV / TNAV** | Tempo que Agrega Valor / Tempo que Não Agrega Valor |
| **SMED / TRF** | Single Minute Exchange of Die / Troca Rápida de Ferramentas — setup em < 10 min |
| **Setup interno** | Ação que exige a máquina parada |
| **Setup externo** | Ação que pode ser feita com a máquina operando |
| **Preset** | Pré-ajuste/pré-montagem de ferramentas fora da máquina |
| **Heijunka** | Nivelamento de produção por volume e mix |
| **Kanban** | Sistema de sinalização para puxar a produção |
| **CONWIP** | Constant Work In Process — controle de WIP por limite fixo |
| **KLT** | Kleinladungsträger — contenedor padrão automotivo (aqui, KLT 4314: 400×300×148 mm, 18 pç) |
| **BIN** | Caixa plástica de armazenagem (NR3, NR4) |
| **Flow rack** | Estante com trilhos roletados para fluxo FIFO por gravidade |
| **FIFO** | First In, First Out |
| **Space buffer** | Pulmão dimensionado por espaço físico (nº de contenedores) |
| **Time buffer** | Pulmão dimensionado por tempo de cobertura |
| **MTS / MTO / ATO** | Make-To-Stock / Make-To-Order / Assembly-To-Order |
| **S&OP** | Sales & Operations Planning |
| **MPS** | Master Production Schedule — Plano Mestre de Produção |
| **MRP** | Material Requirements Planning |
| **PPCP / PPCPM** | Planejamento, Programação e Controle da Produção (e Materiais) |
| **PTF / DTF** | Planning Time Fence / Demand Time Fence — defesas temporais |
| **ATP** | Available To Promise — disponível para promessa |
| **RRC** | Rough Cut Capacity Planning — planejamento agregado de capacidade |
| **CRP** | Capacity Requirements Planning |
| **DRP** | Distribution Requirements Planning |
| **CV** | Coeficiente de Variação = desvio-padrão ÷ média |
| **MAPE** | Mean Absolute Percentage Error — erro percentual absoluto médio da previsão |
| **XYZ** | Classificação por variabilidade: X runner · Y repeater · Z stranger |
| **ABC** | Classificação por valor |
| **CEP** | Controle Estatístico do Processo |
| **MeasurLink** | Software Mitutoyo de coleta e análise de dados de medição |
| **Projeto F4** | Programa de implantação do conceito de célula e medição online em toda a fábrica |
| **Equiptop** | Centro de usinagem multi-pallet (6 peças por pallet) para furo e rosca |
| **Pressmatik** | Prensa de inserção usada na montagem (bucha/porca) |
| **Virada** | Mudança de configuração/produto na linha (3.600 s cada) |
| **Cachimbo** | Componente forjado do terminal de direção (também chamado "caixa") |
| **Pino** | Componente usinado do terminal de direção (esférico) |
| **Master** | Caixa coletiva de embalagem (18 a 21 peças) |
| **Cartucho** | Embalagem individual do produto |
| **TPO** | Trabalho Padrão de Operação |
| **PC** | Plano de Controle |
| **IT** | Instrução de Trabalho |
| **NPU** | Norma de Procedimento de Uso |
| **FO021** | Formulário de registro de inspeção em papel |
| **MOP** | Classificação de movimento (TMP/TOM/TMO) |
| **Tecnicon** | ERP utilizado pela empresa |
| **OP / OC / SC** | Ordem de Produção / Ordem de Compra / Solicitação de Compra |

---

## ANEXO A — TABELAS-FONTE INTEGRAIS

### A.1 Simulação horária completa — cenário base (Rev07, `Planilha3 (2)`)

| Hora | Prod. Pino | WIP a/ Equiptop | Prod. Equiptop | Prod. Caixa 1 | Prod. Caixa 2 | WIP a/ Caixa | Prod. Montagem | WIP a/ Montagem | Prod. Embalagem | WIP a/ Embalagem | Σ Pino | Σ Equiptop | Σ Caixa | Σ Montagem | Σ Embalagem |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 06:00 | 119 | 0 | 119 | 103 | 0 | 16 | 103 | 0 | 103 | 0 | 119 | 119 | 103 | 103 | 103 |
| 07:00 | 119 | 0 | 119 | 103 | 0 | 32 | 103 | 0 | 103 | 0 | 238 | 238 | 206 | 206 | 206 |
| 08:00 | 119 | 0 | 119 | 103 | 0 | 48 | 103 | 0 | 103 | 0 | 357 | 357 | 309 | 309 | 309 |
| 09:00 | 119 | 0 | 119 | 103 | 0 | 64 | 103 | 0 | 103 | 0 | 476 | 476 | 412 | 412 | 412 |
| 10:00 | 119 | 0 | 119 | 103 | 0 | 80 | 103 | 0 | **0** | 103 | 595 | 595 | 515 | 515 | 412 |
| 11:00 | 119 | 0 | 119 | 103 | 0 | 96 | 103 | 0 | **0** | 206 | 714 | 714 | 618 | 618 | 412 |
| 12:00 | 119 | 0 | 119 | 103 | 0 | 112 | **0** | 103 | 188 | 18 | 833 | 833 | 721 | 618 | 600 |
| 13:00 | 119 | 0 | 119 | 103 | 103 | 25 | 125 | 184 | 143 | 0 | 952 | 952 | 927 | 743 | 743 |
| 14:00 | 119 | 0 | 119 | 103 | 41 | 0 | 125 | 203 | 125 | 0 | 1.071 | 1.071 | 1.071 | 868 | 868 |
| 15:00 | 119 | 119 | **0** | **0** | 0 | 0 | 203 | 0 | 188 | 15 | 1.190 | 1.071 | 1.071 | 1.071 | 1.056 |
| 16:00 | 119 | 92 | 146 | 103 | 0 | 43 | 103 | 0 | 118 | 0 | 1.309 | 1.217 | 1.174 | 1.174 | 1.174 |
| 17:00 | 119 | 65 | 146 | 103 | 0 | 86 | 103 | 0 | 103 | 0 | 1.428 | 1.363 | 1.277 | 1.277 | 1.277 |
| 18:00 | 119 | 38 | 146 | 103 | 103 | 26 | 125 | 81 | 125 | 0 | 1.547 | 1.509 | 1.483 | 1.402 | 1.402 |
| 19:00 | 119 | 11 | 146 | 103 | 69 | 0 | 125 | 128 | 125 | 0 | 1.666 | 1.655 | 1.655 | 1.527 | 1.527 |
| 20:00 | 119 | 0 | 130 | 103 | 0 | 27 | 225 | 6 | **0** | 225 | 1.785 | 1.785 | 1.758 | 1.752 | 1.527 |
| 21:00 | 119 | 0 | 119 | 103 | 0 | 43 | **0** | 109 | 188 | 37 | 1.904 | 1.904 | 1.861 | 1.752 | 1.715 |
| 22:00 | 119 | 0 | 119 | 103 | 0 | 59 | 212 | 0 | **0** | 249 | 2.023 | 2.023 | 1.964 | 1.964 | 1.715 |
| 23:00 | 119 | 0 | 119 | 103 | 0 | 75 | 103 | 0 | 188 | 164 | 2.142 | 2.142 | 2.067 | 2.067 | 1.903 |
| 00:00 | 119 | 0 | 119 | 103 | 91 | 0 | 125 | 69 | 188 | 101 | 2.261 | 2.261 | 2.261 | 2.192 | 2.091 |
| 01:00 | 119 | 119 | **0** | **0** | 0 | 0 | 69 | 0 | 170 | 0 | 2.380 | 2.261 | 2.261 | 2.261 | 2.261 |
| 02:00 | 119 | 92 | 146 | 103 | 0 | 43 | 103 | 0 | **0** | 103 | 2.499 | 2.407 | 2.364 | 2.364 | 2.261 |
| 03:00 | 119 | 65 | 146 | 103 | 0 | 86 | 103 | 0 | **0** | 206 | 2.618 | 2.553 | 2.467 | 2.467 | 2.261 |
| 04:00 | 119 | 38 | 146 | 103 | 0 | 129 | **0** | 103 | 188 | 18 | 2.737 | 2.699 | 2.570 | 2.467 | 2.449 |
| 05:00 | 119 | 11 | 146 | 103 | 103 | 69 | 125 | 184 | 143 | 0 | 2.856 | 2.845 | 2.776 | 2.592 | 2.592 |
| 06:00 | 119 | 0 | 130 | 103 | 96 | 0 | 125 | 258 | 125 | 0 | 2.975 | 2.975 | 2.975 | 2.717 | 2.717 |

**Observações críticas:** em **5 das 25 horas** a embalagem fica com produção **zero** (10:00, 11:00, 20:00, 22:00, 02:00, 03:00) enquanto o WIP à sua frente chega a **249 peças**. Em **2 horas** o Equiptop para completamente (15:00 e 01:00). **Isso é starvation e blocking alternados — a assinatura de um sistema não sincronizado.**

### A.2 Matriz completa de cenários de balanceamento

| Atividade | Estado Atual | Balanceado | Balanceado 2 | Método 1 | Método 2 | Novo Layout | Novo Layout 2 | 3 OP Cen 2 | Cen 3 OP | Cenário 1 | Cenário 2 | Cenário 3 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Abast. Pino | 7 | 7 | 7 | 6 | 6 | 6 | 6 | 6 | 6 | 7 | 7 | 7 |
| Abast. Equiptop | 6,67 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 10 | 10 | 10 |
| Abast. Usinagem Caixa | 7 | 7 | 7 | 5,5 | 11 | 11 | 11 | 11 | 11 | 14 | 14 | 14 |
| Abast. Laminação | — | — | — | 0 | 0 | 6 | 6 | 4 | 4 | 4 | 4 | 4 |
| Laminação Rosca | 4 | 4 | 4 | — | — | — | — | — | — | — | — | — |
| Laminação Esfera | 4 | 4 | 4 | 0 | 0 | 0 | 0 | 0 | 0 | — | — | — |
| Inserir Bucha | 8,22 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 |
| Adicionar Graxa | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 |
| Abastecer Pressmatik | 4 | 4 | 4 | 6 | 6 | 6 | 6 | 6 | 6 | 5 | 5 | 5 |
| Inserir Porca | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 |
| Peça no saco plástico | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 |
| Selar o saco | 4,5 | 4,5 | 4,5 | 0 | 0 | 0 | 0 | 4,5 | 4,5 | 4,5 | 4,5 | 4,5 |
| Abrir o cartucho | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 2 |
| Etiquetar | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 |
| Encartuchar | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 |
| Colocar na master | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 |
| Grampear a caixa | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 |
| **Subtotal operação** | **71,42** | **70,53** | **70,53** | **57,53** | **63,03** | **69,03** | **69,03** | **73,28** | **65,28** | **59,03** | **59,03** | **62,03** |
| Atividades de controle | — | 18,65 | 18,65 | — | — | — | — | — | — | — | — | — |
| **TOTAL** | **71,42** | **89,18** | **79,18** | **57,53** | **63,03** | **69,03** | **69,03** | **73,28** | **65,28** | **59,03** | **59,03** | **62,03** |
| **Nº operadores** | 5 | 5 | 5 | 4 | 4 | 4 | 4 | 3 | 3 | 3 | 3 | 3 |
| **Takt (s)** | 30 | 30 | 30 | 28 | 28 | 28 | 28 | 28 | 28 | 28 | 28 | 28 |

### A.3 Resumo financeiro consolidado de todos os investimentos identificados

| Projeto / Item | Valor (R$) | Status |
|---|---|---|
| **MeasurLink TD10** (software, hardware, instrumentos) | **56.419,16** | Aguardando CAPEX |
| — Pacote com 2 licenças | 30.000,00 | |
| — Instrumentos de medição (Fase 1) | 14.979,16 | |
| — Computador completo | 5.000,00 | |
| — Ponto de rede | 2.000,00 | |
| — Licença CAL do servidor | 1.800,00 | |
| — Ponto de energia | 1.200,00 | |
| — Nobreak | 600,00 | |
| — Mesa com suporte para TV | 500,00 | |
| — Leitor de código de barras | 300,00 | |
| — Cabo HDMI | 40,00 | |
| **Fluxo por Família — OCs aprovadas** | **20.810,27** | **APROVADO** |
| — Material elétrico | 4.338,37 | |
| — Nivelamento | 3.707,70 | |
| — Tubo e cantoneira | 2.700,00 | |
| — Movimentação | 2.062,50 | |
| — MO elétrica | 1.890,00 | |
| — Caixa BIN NR4 | 1.668,00 | |
| — MO pneumática | 1.150,00 | |
| — Cofre | 1.119,18 | |
| — Material pneumático | 1.062,00 | |
| — Trilho TR40GP | 572,53 | |
| — Frete | 540,00 | |
| **TOTAL TD10** | **R$ 77.229,43** | |
| | | |
| **Projeto F4 — fábrica completa** | **847.000,00** | Estimado |
| — Família Terminal (TD10+TD20+TD30+TD40) | 180.676,64 | |
| — Família Pivô | 336.598,35 | |
| — Conformação | 137.203,00 | |
| — Família Axial | 106.206,70 | |
| — Tirante/Freio | 86.322,74 | |

---

**FIM DO RELATÓRIO**

*Documento gerado a partir da análise integral de 22 arquivos do repositório `bgdata`. Todos os números apresentados são rastreáveis aos arquivos-fonte citados em cada seção. As divergências entre fontes estão explicitamente registradas na §21 e devem ser resolvidas antes da execução do plano de ação.*
