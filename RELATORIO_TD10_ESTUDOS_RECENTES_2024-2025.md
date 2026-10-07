# RELATÓRIO TÉCNICO — SETOR / LINHA **TD10 (TERMINAL DE DIREÇÃO)**
## Edição restrita aos **estudos mais recentes (abr/2024 – jun/2025)**

| | |
|---|---|
| **Data de emissão deste relatório** | **07/10/2026** |
| **Repositório-fonte** | `FabioVecchia/bgdata` — commit `77adb19` (upload em 07/10/2026) |
| **Critério de corte adotado** | Somente estudos **realizados ou atualizados a partir de 01/01/2024** |
| **Estudos utilizados** | **9 documentos** (abr/2024 a jun/2025) |
| **Documentos descartados por obsolescência** | **13 documentos** (2005 a 2023) |
| **Estudo mais recente da base** | Ferramenta GBO + YAMAZUMI — **13/06/2025** |
| **Estudo mais antigo da base** | GBO TERMINAL — **17/04/2024** |
| **Idade da base de dados** | **1 ano e 4 meses a 2 anos e 6 meses** |

> **Nota metodológica:** todos os números deste relatório são extraídos **exclusivamente** dos 9 documentos listados na §1.1. Nenhum dado dos documentos de 2005–2023 foi utilizado em cálculos, conclusões ou recomendações. A §7 explica item a item o que foi descartado e por quê — incluindo achados importantes sobre a idade real de estudos que vinham sendo tratados como atuais.

---

## ÍNDICE

1. [Critério de recência e inventário datado](#1-critério-de-recência-e-inventário-datado)
2. [Sumário executivo](#2-sumário-executivo)
3. [Estudo a estudo, em ordem cronológica](#3-estudo-a-estudo-em-ordem-cronológica)
   - [3.1 GBO TERMINAL — 17 e 18/04/2024](#31-gbo-terminal--17-e-18042024)
   - [3.2 SHINGO AV/NAV — atualizado 22/05/2024](#32-shingo-avnav--atualizado-22052024)
   - [3.3 Tempos Pressmatik — 01 a 04/07/2024](#33-tempos-pressmatik--01-a-04072024)
   - [3.4 Projeto de Capabilidade / MeasurLink — 06 a 13/08/2024](#34-projeto-de-capabilidade--measurlink--06-a-13082024)
   - [3.5 GBO TD10 Rev06-1 — Estudo de Viradas — 04/05/2025](#35-gbo-td10-rev06-1--estudo-de-viradas--04052025)
   - [3.6 GBO TD10 Rev07 — 08/05/2025](#36-gbo-td10-rev07--08052025)
   - [3.7 Ferramenta GBO + Yamazumi — 13/06/2025](#37-ferramenta-gbo--yamazumi--13062025)
   - [3.8 Trabalho padrão TPO040 e TPO043 — fev e abr/2024](#38-trabalho-padrão-tpo040-e-tpo043--fev-e-abr2024)
4. [Linha do tempo e evolução dos parâmetros](#4-linha-do-tempo-e-evolução-dos-parâmetros)
5. [Diagnóstico consolidado](#5-diagnóstico-consolidado)
6. [Divergências entre os estudos recentes](#6-divergências-entre-os-estudos-recentes)
7. [O que foi descartado e por quê](#7-o-que-foi-descartado-e-por-quê)
8. [Plano de ação](#8-plano-de-ação)
9. [Lacunas e revalidações necessárias](#9-lacunas-e-revalidações-necessárias)
10. [Anexos](#10-anexos)

---

## 1. CRITÉRIO DE RECÊNCIA E INVENTÁRIO DATADO

### 1.1 Estudos UTILIZADOS neste relatório (base de dados oficial)

As datas abaixo foram obtidas dos **metadados internos dos arquivos** (`docProps/core.xml` para Office, metadados PDF, `SummaryInformation` para `.xls`), cruzadas com as datas declaradas no próprio conteúdo.

| # | Estudo | **Data de realização / última atualização** | Autor / responsável | Idade em 07/10/2026 | Natureza do dado |
|---|---|---|---|---|---|
| **E1** | `GBO TERMINAL.xlsx` | **17/04/2024** (criado) → **18/04/2024** (última edição) | Alexandre Kichler Martins | 2 a 5 m | Cronoanálise de 34 eventos, takt, nº de operadores |
| **E2** | `SHINGO - AV NAV.xlsx` | criado 07/04/2022 → **atualizado em 22/05/2024** ⚠ | Alexandre Kichler Martins | 2 a 4 m | Lead time e % de valor agregado |
| **E3** | `Pressmatik/Tempos Pressmatik.xlsx` | **01/07/2024** → **04/07/2024** | Laiza Borges da Silva | 2 a 3 m | Cronoanálise de 4 cenários da Pressmatik |
| **E4** | `01 - PROJETO DE CAPABILIDADE TD10 (MeasurLink).pptx` | declarado "atualizado **06/08/2024**" → salvo **13/08/2024** | Dieferson Duarte Antunes · Paulo Frosi | 2 a 2 m | Investimento, ganhos, fases, Projeto F4 |
| **E5** | `GBO - TD10 - Rev06-1 - ESTUDO DE VIRADAS.xlsx` | criado 11/07/2024 → **04/05/2025** | Matheus de Conto Rodrigues | 1 a 5 m | Revisão anterior do modelo de capacidade |
| **E6** | `Cópia de Cópia de GBO - TD10 - Rev07.xlsx` ⭐ | criado 11/07/2024 → **08/05/2025** | Matheus de Conto Rodrigues | 1 a 5 m | **Modelo vigente**: capacidade, WIP, 10 cenários, perdas |
| **E7** | `Ferramenta GBO + YAMAZUMI - Rev1.xlsm` ⭐ | declarado **03/03/2025** → salvo **13/06/2025** | David Avila Teixeira (Engenharia) | **1 a 4 m** | **Estudo mais recente**: 46 atividades da montagem |
| **E8** | `trabalhopadrao/TPO040.pdf` | **27/02/2024** | — | 2 a 7 m | Trabalho padrão Pino / Torno CNC |
| **E9** | `trabalhopadrao/TPO043.pdf` | Rev. 1 em **01/04/2024** (PDF gerado 03/04/2024) | David Teixeira / Maicon Lemos / José Guedes | 2 a 6 m | Trabalho padrão Embalagem guarda-pó |

⚠ **Ressalva sobre E2 (SHINGO):** o arquivo foi **criado em 07/04/2022** e apenas **atualizado em 22/05/2024**. Não é possível determinar, pelos metadados, se os números de lead time foram recoletados em 2024 ou apenas herdados da versão de 2022. Ele é mantido na base por estar dentro do corte, **mas com confiabilidade rebaixada** — ver §6.3.

### 1.2 Critério de corte

Os 22 arquivos do repositório se separam naturalmente em **dois blocos sem zona cinzenta**:

```
 2005 ─── 2011 ──── 2018 ─── 2021-2023 ────────┊──── 2024 ──── 2025 ── 2026
   │        │         │           │            ┊        │         │
Antropo-   MFV     Workshop   13 documentos    ┊   E1 E2 E3 E4  E5 E6 E7
 metria  335074     + TRF      (fluxo família, ┊   E8 E9
                               layouts, MFV,   ┊
                               setup, TPO41/42)┊
                                               ┊
                                        CORTE: 01/01/2024
                      ◄──── DESCARTADO ────────┊──── UTILIZADO ────►
                            (13 docs)          ┊        (9 docs)
                         3,8 a 21 anos         ┊    1,3 a 2,5 anos
```

Não existe documento entre **21/10/2023** (TPO041/042) e **27/02/2024** (TPO040), o que torna o corte limpo e não arbitrário.

### 1.3 Observação sobre datas de arquivo vs. datas de conteúdo

Dois cuidados foram aplicados para não confundir "data do arquivo" com "data do estudo":

| Caso | Situação | Tratamento |
|---|---|---|
| `GBO Montagem.xlsx` | Conteúdo criado em **10/03/2023**, mas arquivo **re-salvo em 28/09/2026** por Fabio Antonio Dalla Vecchia (9 dias antes do upload ao GitHub) | **Descartado.** A modificação de 2026 é compatível com um simples re-save na preparação do upload; não há nenhuma data interna ou marca de revisão indicando recoleta de dados. **Requer confirmação** — ver §9. |
| `01 - PROJETO DE CAPABILIDADE...pptx` | Arquivo **criado em 25/05/2020** (template herdado), mas conteúdo declarado "atualizado 06.08.24" e salvo em 13/08/2024 | **Utilizado.** A data de criação é do template; o conteúdo é de 2024, confirmado pela base de cálculo declarada (06/2023 a 06/2024). |

---

## 2. SUMÁRIO EXECUTIVO

### 2.1 Os números da base recente

| Indicador | Valor | Estudo | Data |
|---|---|---|---|
| Demanda mensal TD10 | **62.332 peças/mês** | E1 | 04/2024 |
| Dias úteis | 27 | E1 | 04/2024 |
| Demanda por turno | 769,53 peças | E1 | 04/2024 |
| **Takt time TD10** | **37,43 s/peça** | E1 | 04/2024 |
| **Tempo de trabalho manual total** | **59,76 s/peça** | E1 | 04/2024 |
| Nº teórico de operadores | 1,60 → 2 | E1 | 04/2024 |
| **Eficiência medida (março/abril)** | **69,2 %** | E1 | 04/2024 |
| **Gargalo da linha** | **Pino — 30,3 s · 119 pç/h · 2.856 pç/dia** | E6 | 05/2025 |
| **Perdas de disponibilidade** | **28.178 s contra 26.400 s de turno = 106,7 %** | E6 | 05/2025 |
| Takt adotado nos cenários de célula | 28 s e 30 s | E5/E6 | 05/2025 |
| Takt da Pressmatik | 31,5 s | E3 | 07/2024 |
| Takt da montagem (família MTD) | 8,22 s | E7 | 06/2025 |
| Lead time do Terminal | 20.347 min = **14,13 dias** ⚠ | E2 | 05/2024 |
| % de valor agregado (Shingo) | **0,007 %** ⚠ | E2 | 05/2024 |
| Investimento MeasurLink TD10 | **R$ 56.419,16** | E4 | 08/2024 |
| Ganhos quantificados MeasurLink | **R$ 270.283,72** | E4 | 08/2024 |

### 2.2 As seis conclusões da base recente

**1 — A linha não cabe no turno (E6, mai/2025).**
As paradas planejadas somam **28.178 s** contra **26.400 s** de tempo disponível: **razão de 106,7 %**. Se todas as inspeções, viradas, setups e registros fossem executados conforme a norma, **não sobraria um segundo para produzir**. É a explicação estrutural da eficiência de 69,2 % medida em abril/2024.

**2 — 79 % do esforço humano não agrega valor (E1, abr/2024).**
Dos 59,76 s/peça de trabalho manual: **21,2 % AV · 46,7 % NNAV · 32,1 % desperdício puro**. Apenas 12,67 s constroem valor, e as **8 maiores atividades concentram 63,4 % de todo o tempo**.

**3 — O gargalo não tem capacidade nominal para o takt de 2025 (E6).**
A usinagem do pino entrega **2.856 pç/dia** (119 pç/h × 24 h). O takt de **28 s** adotado nos cenários de maio/2025 exige **3.086 pç/dia**. **Déficit de 230 pç/dia (−7,5 %) mesmo a 100 % de eficiência.** No takt de 30 s o déficit é de 0,8 % — a linha opera exatamente no limite, sem qualquer margem.

**4 — Os cenários de 3 operadores de 2025 não são executáveis (E6).**
Recalculando as abas, os cenários de 3 operadores exigem **71,53 a 72,53 s** de carga contra takt de 28 s, resultando em **ocupações máximas de 94,6 % a 99,5 %**. Não há folga para variabilidade. O melhor arranjo real da base recente é o **BALANCEADO (2) com 5 operadores** (89,18 s, ocupação máxima de 74,1 %), que é o **único cenário que inclui as atividades de controle** (18,65 s/peça).

**5 — A montagem pode sair de 5 para 4 postos, mas a proposta está errada (E7, jun/2025).**
O estudo mais recente projeta ganho de **+18,6 % de capacidade** (556 → 659 pç/h) e eliminação de 1 posto. **Porém o posto consolidado OP4 (Cartucho + Master) fica com 10,16 s contra takt de 8,22 s — 23,7 % acima.** A proposta, como está, apenas move o gargalo. A correção é simples e está indicada na §3.7.4.

**6 — O caso de negócio do MeasurLink é sólido (E4, ago/2024).**
**R$ 56.419,16** de investimento contra **R$ 107.770 em ganhos pontuais** (ROI de +91 % no primeiro ciclo) mais **R$ 161.832 em riscos evitados**. E ataca diretamente o item nº 1: **as inspeções são 47,3 % de todas as perdas de disponibilidade**.

### 2.3 A relação entre as seis conclusões

```
        INSPEÇÃO MANUAL + REGISTRO EM PAPEL (FO021)
                        │  13.340 s + 3.360 s por turno
                        ▼
            PERDAS = 106,7 % DO TEMPO DE TURNO          ◄── conclusão 1
                        │
                        ▼
                EFICIÊNCIA DE 69,2 %                     ◄── conclusão 2
                        │
                        ▼
        GARGALO EFETIVO = 2.856 × 0,692 = 1.976 pç/dia
                        │
                        ▼
     DÉFICIT CONTRA A DEMANDA DE 2025 (3.086 pç/dia)     ◄── conclusão 3
                        │
                        ▼
      Impossível reduzir operadores (conclusão 4) ou
      rebalancear a montagem (conclusão 5) ANTES de
      resolver a inspeção → MEASURLINK É O 1º PASSO      ◄── conclusão 6
```

---

## 3. ESTUDO A ESTUDO, EM ORDEM CRONOLÓGICA

---

### 3.1 GBO TERMINAL — **17 e 18/04/2024**

> **Arquivo:** `GBO TERMINAL.xlsx`, aba `TD10`
> **Autor:** Alexandre Kichler Martins
> **Datas:** criado em **17/04/2024 13:53**, última edição em **18/04/2024 16:31**
> **Observação do próprio documento:** *"Dados de Setup e Eficiência coletados referentes aos meses de Março e Abril"* → **coleta de campo em março/abril de 2024**
> **Idade:** 2 anos e 5 meses

#### 3.1.1 Parâmetros

| Parâmetro | Valor | Observação |
|---|---|---|
| Linha | TD10 | |
| **Eficiência março/abril de 2024** | **0,692 (69,2 %)** | medida em campo |
| **Tempo de trabalho manual total** | **59,7627 s/peça** | soma dos 34 eventos |
| **Demanda** | **62.332 peças/mês** | |
| Dias úteis | 27 | |
| Tempo efetivo de operação diária | 28.800 s (8 h) | |
| Demanda por turno | 769,53 peças | 62.332 ÷ 27 ÷ 3 |
| **Takt time** | **37,425 s/peça** | 28.800 ÷ 769,53 |
| **Nº de operadores** | **1,597 → 2** | 59,7627 ÷ 37,425 |

Valores auxiliares da planilha: **109,09 pç/h** · **2.618,18 pç/dia** · **70.690,9 pç/mês** — este último representa a capacidade teórica a 100 % de eficiência, contra 62.332 pç/mês demandados (**folga teórica de 13,4 %**).

#### 3.1.2 Os 34 eventos cronometrados (tabela integral)

| Seq | Operação | Freq. (pç) | Duração (s) | **s/peça** | Classe |
|---|---|---|---|---|---|
| 1 | Deslocamento até o palete de entrada | 450 | 5 | 0,011 | D |
| 2 | Pegar OP | 450 | 4 | 0,009 | D |
| 3 | Deslocamento até o computador | 450 | 15 | 0,033 | D |
| 4 | Mandar imprimir os desenhos técnicos | 450 | 600 | 1,333 | NNAV |
| 5 | Deslocamento até a impressora | 450 | — | 0 | — |
| 4b | Preenchimento de quadro | 80 | 90 | 1,125 | NNAV |
| 5b | Bater caixas trilho gargalo | 216 | 180 | 0,833 | D |
| 6 | Tempo setup Pino | 450 | 594 | 1,320 | NNAV |
| 7 | **Abastecimento máquina Pino** | 1 | 2 | **2,000** | **AV** |
| 8 | Desabastecimento máquina Pino | 1 | 2 | 2,000 | NNAV |
| 9 | **Marcar peça com o marcador industrial** | 1 | 4 | **4,000** | **D** |
| 10 | (evento "2") | 30 | 10 | 0,333 | NNAV |
| 11 | Inspeção Pino micrômetro com registro | 60 | 20 | 0,333 | NNAV |
| 12 | **Inspeção Pino projetor** | 60 | 300 | **5,000** | NNAV |
| 13 | Bater caixa | 18 | 30 | 1,667 | D |
| 14 | **Tempo de setup Equiptop** | 450 | 1.674 | **3,720** | NNAV |
| 15 | Inspeção Equiptop | 50 | 40 | 0,800 | NNAV |
| 16 | **Abastecimento Equiptop** | 6 | 40 | **6,667** | **AV** |
| 17 | Desabastecimento Equiptop | 6 | 15 | 2,500 | NNAV |
| 18 | **Tempo de setup Caixa** | 450 | 1.800 | **4,000** | NNAV |
| 19 | Abastecimento máquina Caixa 1 | 1 | 2 | 2,000 | **AV** |
| 20 | Abastecimento máquina Caixa 2 | 1 | 2 | 2,000 | **AV** |
| 21 | Desabastecimento máquina Caixa 1 | 1 | 2 | 2,000 | NNAV |
| 22 | Desabastecimento máquina Caixa 2 | 1 | 2 | 2,000 | NNAV |
| 23 | Inspeção Caixa cota A e E | 25 | 10 | 0,400 | NNAV |
| 24 | Inspeção Caixa demais cotas | 50 | 20 | 0,400 | NNAV |
| 25 | Bater caixas trilho de saída | 216 | 180 | 0,833 | D |
| 26 | **TEMPO DE DESLOCAMENTO** | 1 | 10 | **10,000** | **D** |
| 27 | Preencher diário de bordo Pino | 100 | 60 | 0,600 | D |
| 28 | Preencher diário de bordo Equiptop | 100 | 60 | 0,600 | D |
| 29 | Preencher diário de bordo Caixa | 100 | 60 | 0,600 | D |
| 30 | Troca de inserto desbaste | 300 | 40 | 0,133 | NNAV |
| 31 | Troca de inserto acabamento | 550 | 180 | 0,327 | NNAV |
| 32 | Trocar ferramenta Equiptop fresa | 6.000 | 180 | 0,030 | NNAV |
| 33 | Troca de ferramenta Equiptop broca | 1.600 | 150 | 0,094 | NNAV |
| 34 | Troca de ferramenta Equiptop macho | 4.000 | 240 | 0,060 | NNAV |
| | **TOTAL** | | | **59,763** | |

*Legenda da própria planilha:* **AV** = Agrega Valor · **NNAV** = Necessário, mas Não Agrega Valor · **D** = Desperdício.

#### 3.1.3 Decomposição do tempo manual

| Classificação | Tempo (s/pç) | % do total |
|---|---|---|
| **AV — Agrega Valor** | **12,667** | **21,2 %** |
| **NNAV — Necessário, não agrega valor** | **27,909** | **46,7 %** |
| **D — Desperdício** | **19,187** | **32,1 %** |
| **TOTAL** | **59,763** | 100 % |

**Apenas 4 das 34 atividades agregam valor** — todas são abastecimento de máquina (pino, Equiptop, caixa 1, caixa 2).

#### 3.1.4 Pareto — as 8 maiores atividades

| Pos. | Atividade | s/pç | % | Classe | Alavanca |
|---|---|---|---|---|---|
| 1 | **Tempo de deslocamento** | 10,000 | 16,7 % | D | Layout / arranjo celular |
| 2 | Abastecimento Equiptop | 6,667 | 11,2 % | AV | Otimizar (não eliminar) |
| 3 | **Inspeção Pino projetor** | 5,000 | 8,4 % | NNAV | **MeasurLink** |
| 4 | Marcar peça com marcador industrial | 4,000 | 6,7 % | D | Marcação a laser / poka-yoke |
| 5 | Tempo de setup Caixa | 4,000 | 6,7 % | NNAV | SMED |
| 6 | Tempo de setup Equiptop | 3,720 | 6,2 % | NNAV | SMED |
| 7 | Desabastecimento Equiptop | 2,500 | 4,2 % | NNAV | Automação de descarga |
| 8 | Abastecimento máquina Pino | 2,000 | 3,3 % | AV | Otimizar |
| | **Subtotal** | **37,887** | **63,4 %** | | |

> **63,4 % de todo o tempo manual está em 8 atividades.** Eliminando apenas as de classe **D** entre elas (deslocamento 10 s + marcação 4 s = 14 s), o tempo manual cairia para **45,76 s** e o nº de operadores de 1,60 para **1,22**.

#### 3.1.5 Cenários derivados

| Cenário | Tempo manual | Nº de operadores | Viabilidade |
|---|---|---|---|
| **Atual (abr/2024)** | 59,76 s | **1,60 → 2** | Opera com 2 |
| Eliminando todo o desperdício (D) | 40,58 s | **1,08 → 2** | Ainda exige 2, com 46 % de ociosidade no 2º |
| Eliminando D + metade do NNAV | 26,62 s | **0,71 → 1** | **1 operador com 29 % de folga** |

---

### 3.2 SHINGO AV/NAV — **atualizado 22/05/2024**

> **Arquivo:** `SHINGO - AV NAV.xlsx`, aba `SHINGO - F3`
> **Autor:** Alexandre Kichler Martins
> **Datas:** criado em **07/04/2022**, última edição em **22/05/2024 11:03**
> **Idade (última atualização):** 2 anos e 4 meses
> ⚠ **Confiabilidade rebaixada** — ver ressalva ao final desta seção

#### 3.2.1 Resultado: porcentagem de valor agregado (Terminal)

| Símbolo / Atividade | Agrega valor? | TAV (min) | TNAV (min) | % do Lead Time |
|---|---|---|---|---|
| Estoque de matéria-prima | N | — | 0 | 0 % |
| Transporte | N | — | 6 | 0,0295 % |
| **Esperando processo** | N | — | **19.980** | **98,19 %** |
| **PROCESSANDO** | **S** | **1,43** | — | **0,00703 %** |
| Esperando lote | N | — | 360 | 1,769 % |
| Inspeção | N | — | 0 | 0 % |
| Estoque de produto | N | — | 0 | 0 % |
| **TOTAL** | | **1,43 min** | **20.346 min** | |

| Indicador | Valor |
|---|---|
| **Lead Time Total** | **20.347,43 min** |
| **Lead Time Total** | **339,12 horas** |
| **Lead Time Total** | **14,13 dias** |
| **% de valor agregado** | **0,00703 %** |

Contadores de ocorrências registrados na planilha (colunas d/h/t/e/l/P): **86 eventos** no total, com valores complementares de **39 / 6 / 18 / 63**.

#### 3.2.2 Leitura

> **Para 1,43 minuto de processamento efetivo, o produto passa 14,13 dias no sistema.** **98,19 % do lead time é espera por processamento** — fila entre operações, não tempo de máquina.

Isso caracteriza um problema de **sincronização e tamanho de lote**, não de velocidade de equipamento. Nenhuma melhoria de tempo de ciclo no TD10 altera materialmente esse número: reduzir o processamento de 1,43 min para 0,7 min mudaria o lead time em **0,0035 %**.

#### 3.2.3 ⚠ Ressalva de confiabilidade

| Ponto | Situação |
|---|---|
| Criação do arquivo | 07/04/2022 — **fora do corte** |
| Última modificação | 22/05/2024 — **dentro do corte** |
| Evidência de recoleta em 2024 | **Nenhuma** nos metadados ou no conteúdo |
| Risco | Os números podem ter sido **herdados** da versão de 2022 e o arquivo apenas reaberto/ajustado em 2024 |

**Tratamento adotado:** o estudo é apresentado por estar formalmente dentro do corte, mas **é o único da base cujo dado não deve embasar decisão de investimento sem revalidação**. A §9 inclui a revalidação do lead time como ação prioritária.

---

### 3.3 Tempos Pressmatik — **01 a 04/07/2024**

> **Arquivo:** `Pressmatik/Tempos Pressmatik.xlsx`
> **Autora:** Laiza Borges da Silva
> **Datas:** criado em **01/07/2024 14:20**, última edição em **04/07/2024 14:04**
> **Idade:** 2 anos e 3 meses
> **Método:** cronometragem direta de ciclos completos em 4 arranjos distintos

#### 3.3.1 CENÁRIO 1 — 13 ciclos cronometrados

| Elemento | Tempo médio (s) | Mínimo | Máximo | Amplitude |
|---|---|---|---|---|
| Operação Pressmatik | **10,955** | 10,00 | 13,58 | 36 % |
| Porca | **5,707** | 3,72 | 10,60 | 185 % |
| Saquinho | **7,613** | 5,89 | 9,61 | 63 % |
| Caixinha | **7,716** | 6,90 | 8,87 | 29 % |
| Etiqueta (medição separada, 10 ciclos) | 4,604 | 3,14 | 6,63 | 111 % |
| Bucha (medição separada) | 8,220 | — | — | — |
| Ciclo montagem master | 0,830 | — | — | — |
| Ciclo finalização master | 1,234 | — | — | — |
| **TEMPO TOTAL DE OPERAÇÃO** | **46,875 s** | | | |

#### 3.3.2 CENÁRIO 3 — 6 ciclos

| Elemento | Tempo médio (s) |
|---|---|
| Bucha | 8,218 |
| **Operação Pressmatik** | **2,707** (−75 % vs. Cenário 1) |
| Porca | 4,855 |
| Saquinho | 8,503 |
| **Caixinha** | **15,802** (+105 % vs. Cenário 1) |
| Ciclo montagem master | 0,830 |
| Ciclo finalização master | 1,234 |
| **TEMPO TOTAL** | **42,149 s** |

#### 3.3.3 CENÁRIO 4 — 10 ciclos

| Elemento | Tempo médio (s) |
|---|---|
| Bucha | 8,916 |
| Operação Pressmatik | 2,457 |
| Saquinho | 9,779 |
| Caixinha | 12,941 |
| Ciclo montagem master | 0,830 |
| Ciclo finalização master | 1,234 |
| **TEMPO TOTAL** | **36,157 s** |

#### 3.3.4 CENÁRIO 5 — 6 ciclos — **melhor resultado**

| Elemento | Tempo médio (s) |
|---|---|
| Operação Pressmatik | 9,753 |
| Saquinho | 10,222 |
| Caixinha | 12,220 |
| Ciclo montagem master | 0,830 |
| Ciclo finalização master | 1,234 |
| **TEMPO TOTAL** | **34,259 s** |

Tempos totais individuais registrados neste cenário: **28,83 s · 27,60 s · 32,46 s** — variabilidade de ±8 % no ciclo completo.

#### 3.3.5 Comparação final (aba `COMPARAÇÃO`)

| | Cenário 1 | Cenário 3 | Cenário 4 | **Cenário 5** |
|---|---|---|---|---|
| **Tempo de ciclo (s)** | 46,88 | 42,15 | 36,16 | **34,26** |
| **Entrega (pç/h)** | 76,79 | 85,41 | 99,56 | **105,08** |
| **Ganho acumulado** | — | +11,2 % | +29,6 % | **+36,8 %** |

| Fechamento do estudo | Valor |
|---|---|
| **Melhor tempo de ciclo** | **34,26 s** |
| **Takt alvo** | **31,50 s** |
| **GAP remanescente** | **2,76 s (8,8 % acima do takt)** ⚠ |

**Medições da caixa master:**

| | Montagem master | Finalização master |
|---|---|---|
| Medição 1 | 14,91 s | 23,60 s |
| Medição 2 | 14,96 s | 20,83 s |
| **Média** | **14,935 s** | **22,215 s** |
| **Rateado (18 pç/caixa)** | **0,830 s/pç** | **1,234 s/pç** |

#### 3.3.6 Leitura

O estudo entregou **+36,8 % de produtividade** (76,8 → 105,1 pç/h), mas **não fechou o takt**: faltam **2,76 s**. O elemento **"Caixinha"** é o maior do cenário vencedor (12,22 s) e o mais instável de todo o estudo — variou de **7,72 s → 15,80 s → 12,94 s → 12,22 s** entre cenários (amplitude de 105 %).

> **Conclusão:** o gap de 2,76 s está integralmente dentro da variabilidade do encartuchamento. **Padronizar esse único elemento fecha o takt sem investimento.**

---

### 3.4 Projeto de Capabilidade / MeasurLink — **06 a 13/08/2024**

> **Arquivo:** `01 - PROJETO DE CAPABILIDADE TD10 ( Measure Link ) - atualizado 06.08.24.pptx`
> **Responsáveis:** Paulo Frosi · Dieferson Duarte Antunes
> **Datas:** título declara "atualizado **06/08/2024**"; arquivo salvo em **13/08/2024 08:57** (template-base criado em 2020)
> **Base de cálculo dos ganhos:** **06/2023 a 06/2024** (12 meses de histórico real)
> **Idade:** 2 anos e 2 meses

#### 3.4.1 Objetivo declarado

> *"Implementar um sistema de medição online avançado para inspeção de peças fabricadas na usinagem, proporcionando controle estatístico do processo em tempo real, aumento de eficiência devido à maior disponibilidade do operador, precisão nas medições, eliminação do uso de registros em papel, bem como a **redução de 30 % da sucata operacional** gerada na linha TD10, assegurando que as peças sejam fabricadas corretamente na primeira vez, servindo como base para os projetos **"F4"** e **"Rumo ao Defeito Zero"**."*

#### 3.4.2 Mudança de modelo

| Etapa | Modelo ATUAL | Modelo PROPOSTO |
|---|---|---|
| 1 | Abertura do registro de inspeção em papel (**FO021**) | Abertura automática no MeasurLink |
| 2 | Inspeção com instrumentos analógicos | Instrumentos digitais com transmissão de dados |
| 3 | Registro manual dos dados | Registro automático |
| 4 | Fechamento manual | Fechamento no sistema |
| 5 | Arquivamento físico em caixas | Arquivamento digital |

#### 3.4.3 Fases

| Fase | Escopo | Prazo |
|---|---|---|
| **1ª** | Efetivação na **máquina gargalo do TD10** | **15 dias** após liberação do CAPEX |
| **2ª** | Linha TD10 completa | **90 dias** após liberação do CAPEX |
| **3ª** | Demais células, conforme avanço do Projeto F4 | Conforme avanço |

> Atacar primeiro o gargalo é a decisão correta pela Teoria das Restrições: hora ganha no gargalo é hora ganha no sistema inteiro.

#### 3.4.4 Investimento — detalhamento integral

**Piloto:** 45 dias **sem custo**, sistema cedido pelo representante Mitutoyo.

| Item | Qtd | Valor (R$) |
|---|---|---|
| Pacote com 2 licenças | 1 | 30.000,00 |
| Equipamentos e instrumentos de medição | 1 | 14.979,16 |
| Computador completo | 1 | 5.000,00 |
| Ponto de rede | 1 | 2.000,00 |
| Licença CAL do servidor | 1 | 1.800,00 |
| Ponto de energia | 1 | 1.200,00 |
| Nobreak | 1 | 600,00 |
| Mesa com suporte para TV | 1 | 500,00 |
| Leitor de código de barras | 1 | 300,00 |
| Cabo HDMI | 1 | 40,00 |
| **TOTAL** | | **R$ 56.419,16** |

**Instrumentos de medição — Fase 1:**

| Qtd | Instrumento | Custo (R$) |
|---|---|---|
| 1 | Paquímetro 150 | 3.046,54 |
| 1 | Micrômetro externo 0–25 | 3.278,52 |
| 1 | Micrômetro externo 25–50 | 4.104,83 |
| 1 | Paquímetro 300 | 4.549,27 |
| | **TOTAL** | **14.979,16** |

**Suporte técnico:**

| Fornecedor | Modalidade | Custo |
|---|---|---|
| Mitutoyo (software) | Presencial | R$ 180/h + deslocamento |
| Mitutoyo (software) | **Remoto** | **Gratuito por tempo indeterminado** |
| 3D Metrologia (ferramental) | Presencial | R$ 150/h + deslocamento |
| 3D Metrologia (ferramental) | **Remoto** | **Gratuito por tempo indeterminado** |

**Requisitos de sistema:**

| Categoria | Requisito |
|---|---|
| SGBD | Microsoft SQL Server 2014 / 2016 / 2017 (Standard ou Enterprise) |
| Sistema operacional | Windows 8 (exceto RT) e Windows 10 (exceto Mobile/IoT), 32 e 64 bits |
| Processador | 1 GHz ou superior (x86 ou x64) |
| Memória | 4 GB (32 bits) · 8 GB (64 bits) |
| Disco | 16 GB (32 bits) · 20 GB (64 bits) |
| Vídeo | DirectX 9 com WDDM 1.0 ou superior |

> ⚠ Os requisitos citam SQL Server 2014/2016/2017 e Windows 8/10 — **tecnologias já em fim de suporte em 2026**. A especificação precisa ser revalidada com o fornecedor antes da compra (§9).

#### 3.4.5 Ganhos tangíveis (base 06/2023 – 06/2024)

| Ganho | Tipo | Fator | Valor base (R$) | **Considerado (R$)** |
|---|---|---|---|---|
| Redução do nº de sucata operacional > 1 peça (TD10) | Ganho pontual | 1 | 2.170,00 | **2.170,00** |
| Aderência ao MPS — perdas com desvio e retrabalho (Gargalo) | Risco evitado | 0,25 | 246.576,00 | **61.644,00** |
| Aderência ao MPS — sucata operacional (Gargalo) | Ganho mensal constante | 1 | 418,00 | **418,00** |
| Aderência ao MPS — desvios e retrabalho (Equiptop e caixa) | Risco evitado | 1 | 88.660,00 | **88.660,00** |
| Aderência ao MPS — sucata operacional (Equiptop e caixa) | Risco evitado | 1 | 11.528,00 | **11.528,00** |
| Redução de custos com papel físico (FO021) | Ganho mensal constante | 1 | 42,12 | **42,12** |
| Redução de caixas de arquivamento | Ganho mensal constante | 1 | 2,60 | **2,60** |
| Aderência ao MPS — estudos de capabilidade (24 h → 4 h) | Ganho pontual | 1 | 105.600,00 | **105.600,00** |
| Redução no custo de calibração externa | Ganho mensal constante | 2 | 109,50 | **219,00** |
| | | | **TOTAL** | **R$ 270.283,72** |

**Por natureza:**

| Natureza | Valor |
|---|---|
| **Ganhos pontuais** | **R$ 107.770,00** |
| **Riscos evitados** | **R$ 161.832,00** |
| **Ganhos mensais constantes** | **R$ 681,72/mês** (R$ 8.180,64/ano) |

**Retorno:** R$ 107.770 de ganho pontual contra R$ 56.419,16 de investimento → **ROI de +91 % no primeiro ciclo**, payback inferior a 12 meses. Com riscos evitados, o retorno total é de **4,8× o investimento**.

#### 3.4.6 Base de cálculo detalhada

**a) Redução de 50 % de sucatas > 1 peça** (total de 376 peças em 12 meses):

| Item | Peças | Valor unit. | Total |
|---|---|---|---|
| Pino | 57 | R$ 3,60 | R$ 205,20 |
| Cachimbo | 131 | R$ 15,00 | R$ 1.965,00 |
| | | **TOTAL** | **R$ 2.170,20** |

**b) Faturamento não realizado por sucatas > 1 peça** (376 peças):

| Item | Peças | Valor unit. | Total |
|---|---|---|---|
| Pino | 114 | R$ 44,00 | R$ 5.016,00 |
| Cachimbo | 262 | R$ 44,00 | R$ 11.528,00 |
| | | **TOTAL** | **R$ 16.544,00** |

**c) Faturamento fora do prazo por retrabalhos e desvios** (9.425 peças):

| Item | Peças | Valor unit. | Total |
|---|---|---|---|
| Pino | 1.401 | R$ 44,00 | R$ 61.644,00 |
| Cachimbo | 575 | R$ 44,00 | R$ 25.300,00 |
| | | **TOTAL** | **R$ 86.944,00** |

**d) Redução de máquina parada por estudos de capabilidade:**

| | Atual | Proposto |
|---|---|---|
| Tempo médio de parada | **24 h** | **4 h** |
| Impacto no gargalo | 3.072 peças | 512 peças |
| Produção horária do gargalo considerada | **128 pç/h** ⚠ | 128 pç/h |
| Impacto no faturamento | − R$ 135.168 | − R$ 22.528 |
| **GANHO por máquina** | | **R$ 112.640** |

⚠ Este estudo adota **128 pç/h** para o gargalo, enquanto o E6 (mai/2025) registra **119 pç/h** — ver §6.1.

#### 3.4.7 Ganhos intangíveis declarados

1. Capabilidade do processo em tempo real (gestão visual).
2. Rapidez na tomada de decisão baseada em análise estatística imediata.
3. Melhoria na exatidão das medições — mitigação de erros de transcrição e interpretação.
4. **Redução de 50 % no número de instrumentos utilizados.**
5. Disponibilidade dos dados em tempo real (informação documentada — requisito de norma).
6. Alerta na tela e disparo de e-mail para peça fora de tolerância.
7. **Possibilidade de bloqueio de máquina** por peça fora de tolerância ou por medição não realizada no período estipulado.
8. **Redução de 3 minutos no tempo de medição** (setup e troca de OP).

#### 3.4.8 Riscos declarados

| Risco | Mitigação disponível |
|---|---|
| Gestão da mudança | Engajamento dos operadores (declarado no escopo) |
| Má utilização dos equipamentos | Treinamento (Gente e Cultura) |
| Falha na coleta ou perda de dados por falta de energia | **Nobreak já orçado** |
| Custo adicional para interligação software ↔ máquina (bloqueio do CNC) | Não orçado — **risco financeiro aberto** |
| Interligação de outros meios de medição (outros fabricantes) | Não endereçado |

#### 3.4.9 Projeto F4 — mapa de investimento da fábrica

| Família | Células | Valor unitário (R$) | **Subtotal (R$)** |
|---|---|---|---|
| **Terminal** | **TD10** | **56.419,16** | |
| | TD20 · TD30 · TD40 | 41.419,16 cada | **180.676,64** |
| **Pivô** | PA10–PA40 · PC10–PC40 · JS (parcial) | 36.869,89 / 41.639,27 | **336.598,35** |
| **Conformação** | — | — | **137.203,00** |
| **Axial** | JS10 · JS20 | 36.869,89 | **106.206,70** |
| **Tirante/Freio** | TE10/1 (39.915,87) · TE10/2 (46.406,87) | | **86.322,74** |
| | | **TOTAL ESTIMADO** | **R$ 847.000,00** |

*Legenda de status do slide:* Em andamento · Não iniciado · Conceito de célula não implementado.
*Observação do documento:* "Sem cotação com outros fornecedores."

> O **TD10 tem o maior investimento unitário (R$ 56.419,16)** porque carrega o pacote de licenças e o servidor — as demais células herdam a infraestrutura. **É o investimento habilitador de todo o Projeto F4.**

#### 3.4.10 Árvore de benefícios

```
                  MEASURLINK – TD10
    ┌──────────┬──────────┬──────────┬──────────┐
    ▼          ▼          ▼          ▼          ▼
 Reduzir    Mudança   Fazer certo  Eficiência  Redução do
 30 % da    de        na primeira  operacional tempo NAV
 sucata     cultura   vez                      (FO021)
    └──────────┴──────────┴──────────┴──────────┘
                         ▼
          RUMO AO DEFEITO ZERO   ·   PROJETO F4
                         ▼
                   INDÚSTRIA 4.0
```

---

### 3.5 GBO TD10 Rev06-1 — Estudo de Viradas — **04/05/2025**

> **Arquivo:** `GBO - TD10 - Rev06-1 - ESTUDO DE VIRADAS - DIA A DIA.xlsx`
> **Autor:** Matheus de Conto Rodrigues
> **Datas:** criado em **11/07/2024**, última edição em **04/05/2025 20:11**
> **Idade:** 1 ano e 5 meses
> **Status:** **revisão anterior**, superada pela Rev07 (08/05/2025, 4 dias depois)

#### 3.5.1 O que esta revisão contém de exclusivo

A Rev06-1 traz **duas abas de cenário que não existem na Rev07**: `NOVO LAYOUT` e `NOVO LAYOUT (2)`, ambas com 4 operadores e takt de 28 s.

**NOVO LAYOUT:**

| Atividade | Op1 | Op2 | Op3 | Op4 |
|---|---|---|---|---|
| Abastecimento Pino | 6,00 | | | |
| Abastecimento Equiptop | | 12,00 | | |
| Abastecimento Usinagem Caixa | | 11,00 | | |
| Abastecimento Laminação | 6,00 | | | |
| Inserir Bucha | | | 2,00 | |
| Adicionar Graxa | | | 2,00 | |
| Abastecer Pressmatik | | | 6,00 | |
| Inserir Porca | | | 4,86 | |
| Peça no saco plástico | | | | 4,00 |
| Abrir o cartucho | | | | 2,00 |
| Etiquetar | | | | 4,00 |
| Encartuchar | | | | 5,25 |
| Colocar na master | | | | 2,25 |
| Grampear a caixa | | | | 1,67 |
| **Total** | **12,00** | **23,00** | **14,86** | **19,17** |
| **Ocupação (takt 28 s)** | 42,9 % | **82,1 %** | 53,1 % | 68,5 % |
| | | **Carga total: 69,03 s** | | |

**NOVO LAYOUT (2):** mesma carga total de **69,03 s**, com redistribuição — Op1 12,00 · Op2 20,00 · Op3 13,00 · Op4 24,03 · ocupação máxima **85,8 %**.

#### 3.5.2 Comparação Rev06-1 → Rev07

| Aba | Rev06-1 (04/05/2025) | Rev07 (08/05/2025) | Delta |
|---|---|---|---|
| Cenários de 4 operadores | NOVO LAYOUT · NOVO LAYOUT (2) — **69,03 s** | MÉTODO 1 (**57,53 s**) · MÉTODO 2 (**63,03 s**) | **−6,0 a −11,5 s** |
| Abastecimento Laminação | **6,00 s** incluído | **0,00 s** (removido do escopo) | −6,00 s |
| Abastecimento Usinagem Caixa | 11,00 s | 5,50 s (Método 1) / 11,00 s (Método 2) | −5,50 s no Método 1 |
| Abas de capacidade | `Planilha3 (2)` e `(3)` | idem + `Planilha4` e `CONSOLIDAÇÃO` | Rev07 mais completa |

> **Interpretação da evolução:** entre 04 e 08/05/2025 o estudo evoluiu em dois pontos — **(a)** o abastecimento da laminação (6 s) saiu do escopo da célula e **(b)** criou-se a distinção entre operar **com** e **sem** WIP de caixa (Métodos 1 e 2). A Rev07 é, portanto, a versão vigente e é ela que embasa a §3.6.

---

### 3.6 GBO TD10 Rev07 — **08/05/2025** ⭐ MODELO VIGENTE

> **Arquivo:** `Cópia de Cópia de GBO - TD10 - Rev07.xlsx`
> **Autor:** Matheus de Conto Rodrigues
> **Datas:** criado em **11/07/2024**, última edição em **08/05/2025 12:42**
> **Idade:** 1 ano e 5 meses
> **Conteúdo:** 18 abas — capacidades, simulação horária de WIP, 10 cenários de balanceamento, perdas de disponibilidade
> ⚠ O repositório contém **duas cópias byte-idênticas** deste arquivo (MD5 `0303913a41a23d4007bc15ff4d509952`): `Cópia de Cópia de...` e `!!Cópia de Cópia de...`

#### 3.6.1 Capacidade por operação

**Cenário-base (aba `Planilha3 (2)`):**

| Operação | Tempo de ciclo (s) | Capacidade (pç/h) | Horas operando | Capacidade disponível (pç) |
|---|---|---|---|---|
| **PINO** | **30,3** | **118,8** | 24 | 2.851,5 |
| CAIXA (máq. 1) | 35,0 | 102,9 | 21 | 2.160,0 |
| CAIXA (máq. 2) | 35,0 | 102,9 | **0** | 0 |
| EQUIPTOP | 24,7 | 145,7 | 21 | 3.060,7 |
| MONTAGEM | 14,86 | 242,3 | 15 | 3.633,9 |
| EMBALAGEM | 19,1 | 188,5 | 21 | 3.958,1 |

**Cenário expandido (aba `Planilha3 (3)`):**

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

**Capacidade consolidada (aba `Planilha4`):**

| Operação | Capacidade/h | Horas produtivas | **Capacidade total/dia** |
|---|---|---|---|
| **PINO** | **119** | 24 | **2.856** ← menor |
| EQUIPTOP | 146 | 21 | 3.066 |
| CAIXA (2 máq.) | 206 | 21 | 4.326 |
| MONTAGEM | 150 | 21 | 3.150 |
| EMBALAGEM | 150 | 21 | 3.150 |

#### 3.6.2 ⚠ O gargalo não suporta o takt adotado

Os cenários desta mesma planilha adotam takt de **28 s** (maioria) e **30 s** (estado atual e balanceados). Confrontando com a capacidade do pino:

| Takt adotado | Demanda implícita (24 h) | Capacidade do pino | **Situação** |
|---|---|---|---|
| **28 s** | **3.085,7 pç/dia** | 2.856 pç/dia | **Déficit de 229,7 pç/dia (−7,4 %)** ❌ |
| **30 s** | **2.880,0 pç/dia** | 2.856 pç/dia | **Déficit de 24 pç/dia (−0,8 %)** ⚠ |

> **Achado crítico:** no takt de 28 s, **a usinagem do pino não atende a demanda nem a 100 % de eficiência**. No takt de 30 s, atende com 0,8 % de déficit — ou seja, **margem zero**. Aplicando a eficiência medida de 69,2 % (E1), a capacidade efetiva cai para **1.976 pç/dia**, um **déficit de 36 %** contra o takt de 28 s.
>
> **Consequência:** qualquer cenário de balanceamento desta planilha pressupõe uma capacidade de gargalo que a própria planilha mostra não existir. **Antes de rebalancear operadores, é preciso liberar capacidade no pino.**

#### 3.6.3 PERDAS DE DISPONIBILIDADE — o achado central

| Atividade | Tempo unitário (s) | Repetições/turno | **Tempo total (s)** | % |
|---|---|---|---|---|
| Inspeção caixa (1/50) | 102 | 20 | 2.040 | 7,2 % |
| Inspeção caixa (1/25) | 29 | 40 | 1.160 | 4,1 % |
| Inspeção Equiptop (1/50) | 106 | 20 | 2.120 | 7,5 % |
| **Inspeção montagem** | **1.000** | **7** | **7.000** | **24,8 %** |
| Inspeção pino (1/60) | 60 | 17 | 1.020 | 3,6 % |
| **Virada 1** | 3.600 | 1 | **3.600** | **12,8 %** |
| **Virada 2** | 3.600 | 1 | **3.600** | **12,8 %** |
| Preencher diário de bordo | 60 | 48 | 2.880 | 10,2 % |
| Preencher quadro | 60 | 8 | 480 | 1,7 % |
| Setup Pino | 720 | 1 | 720 | 2,6 % |
| Setup Equiptop | 1.758 | 1 | 1.758 | 6,2 % |
| Setup Caixa | 1.800 | 1 | 1.800 | 6,4 % |
| **TOTAL DE PERDAS** | | | **28.178 s** | 100 % |
| **Tempo disponível por turno** | | | **26.400 s** | |
| **RAZÃO** | | | **1,0673 → 106,7 %** | |

**Agrupamento por bloco:**

| Bloco | Tempo (s) | % das perdas | Projeto que ataca |
|---|---|---|---|
| **Inspeções (5 tipos)** | **13.340** | **47,3 %** | **MeasurLink (E4)** |
| **Viradas (2)** | **7.200** | **25,6 %** | Nivelamento / redução de setup |
| **Setups (3)** | **4.278** | **15,2 %** | SMED |
| **Registros (diário + quadro)** | **3.360** | **11,9 %** | **MeasurLink (E4)** |
| **TOTAL** | **28.178** | 100 % | |

> **A inspeção da montagem (7.000 s) sozinha é 24,8 % de todas as perdas.** O MeasurLink, atacando inspeções + registros, endereça **16.700 s = 59,2 % das perdas**.
>
> **Simulação:** eliminando metade do bloco endereçável pelo MeasurLink (8.350 s), a razão cai de **106,7 % para 75,1 %** — liberando ~31,6 pontos percentuais de tempo produtivo.

**Visão alternativa (aba `Planilha2`):**

| Parada | Tempo (s) |
|---|---|
| Setup Pino | 1.800 |
| **Virada** | **10.800** |
| Inspeção Pino | 1.600 |
| Inspeção Caixa | 1.600 |
| Inspeção Equiptop | 1.600 |
| Inspeção Laminação | 1.600 |
| Montagem | 1.600 |
| **Total** | **20.600** (referência de 25.200 s) |

⚠ Divergência interna ao mesmo arquivo: a virada vale **7.200 s** numa aba e **10.800 s** noutra — ver §6.2.

#### 3.6.4 Cenários de balanceamento — **valores recalculados célula a célula**

> Os valores abaixo foram recalculados diretamente das células de cada aba, somando as colunas de operador e dividindo pelo takt declarado na própria aba.

| Cenário | Nº op. | Takt (s) | **Carga total (s)** | Cargas por operador (s) | Ocup. média | **Ocup. máxima** | Inclui controle? |
|---|---|---|---|---|---|---|---|
| **ESTADO ATUAL** | 5 | 30 | **71,42** | 8,67 · 6,67 · 7,00 · 8,00 · **41,08** | 47,6 % | **136,9 %** ❌ | Não |
| **BALANCEADO** | 5 | 30 | **89,18** | 23,75 · **1,36** · 16,41 · 25,66 · 22,00 | 59,5 % | 85,5 % | **Sim** |
| **BALANCEADO (2)** ⭐ | 5 | 30 | **89,18** | 11,75 · 22,22 · 20,41 · 18,80 · 16,00 | 59,5 % | **74,1 %** ✅ | **Sim** |
| MÉTODO 1 | 4 | 28 | **57,53** | 6,00 · 19,50 · 12,86 · 19,17 | 51,4 % | 69,6 % | Não |
| MÉTODO 2 (com WIP CX) | 4 | 28 | **63,03** | 6,00 · 20,00 · 13,00 · 24,03 | 56,3 % | 85,8 % | Não |
| NOVO LAYOUT – 3 OP CEN 2 | 3 | 28 | **71,53** | 20,86 · 23,67 · 27,00 | 85,2 % | **96,4 %** ❌ | Não |
| NOVO LAYOUT CENÁRIO 3 OP | 3 | 28 | **71,53** | 21,17 · 26,50 · 23,86 | 85,2 % | **94,6 %** ❌ | Não |
| CENÁRIO 1 | 3 | 28 | **72,53** | 26,67 · 27,86 · 18,00 | 86,3 % | **99,5 %** ❌ | Não |
| CENÁRIO 2 | 3 | 28 | **72,53** | 26,67 · 23,86 · 22,00 | 86,3 % | **95,2 %** ❌ | Não |
| CENÁRIO 3 | 3 | 28 | **72,53** | 26,67 · 19,86 · 26,00 | 86,3 % | **95,2 %** ❌ | Não |

#### 3.6.5 Detalhamento do ESTADO ATUAL (5 operadores, takt 30 s)

| Atividade | Op. Pino | Op. Equiptop | Op. Caixa | Op. Laminação | Op. Montagem |
|---|---|---|---|---|---|
| Abastecimento Pino | 7,00 | | | | |
| Abastecimento Equiptop | | 6,67 | | | |
| Abastecimento Usinagem Caixa | | | 7,00 | | |
| Laminação Rosca | | | | 4,00 | |
| Laminação Esfera | | | | 4,00 | |
| **Inserir Bucha** | | | | | **8,22** |
| Adicionar Graxa | | | | | 2,00 |
| Abastecer Pressmatik | | | | | 4,00 |
| Inserir Porca | | | | | 4,86 |
| Peça no saco plástico | | | | | 4,00 |
| Selar o saco | | | | | 4,50 |
| Abrir o cartucho | | | | | 2,00 |
| Etiquetar | | | | | 4,00 |
| Encartuchar | | | | | 5,25 |
| Colocar na master | | | | | 2,25 |
| Grampear a caixa | 1,67 | | | | |
| **CARGA (s)** | **8,67** | **6,67** | **7,00** | **8,00** | **41,08** |
| **OCUPAÇÃO** | 28,9 % | 22,2 % | 23,3 % | 26,7 % | **136,9 %** ❌ |

> **Desbalanceamento extremo:** o Operador de Montagem carrega **57,5 % de toda a célula sozinho** e opera **37 % acima do takt**, enquanto os outros quatro somam **30,34 s** e ficam abaixo de 29 % de ocupação. Há **~89 s de ociosidade por ciclo** distribuídos em 4 pessoas.

#### 3.6.6 Detalhamento do BALANCEADO (2) — **melhor cenário real da base**

Este é o **único cenário da Rev07 que inclui as atividades de controle**, o que o torna o único comparável à realidade operacional.

| Atividade | Op. Pino | Op. Equiptop | Op. Caixa | Op. Laminação | Op. Montagem |
|---|---|---|---|---|---|
| Abastecimento Pino | 7,00 | | | | |
| Abastecimento Equiptop | | 12,00 | | | |
| Abastecimento Usinagem Caixa | | | 7,00 | | |
| Laminação Rosca / Esfera | | | | 4,00 + 4,00 | |
| Inserir Bucha | | | 2,00 | | |
| Adicionar Graxa | | | 2,00 | | |
| Abastecer Pressmatik | | | | | 4,00 |
| Inserir Porca | | 4,86 | | | |
| Peça no saco plástico | | 4,00 | | | |
| Selar o saco | | | | | 4,50 |
| Abrir o cartucho | | | | 2,00 | |
| Etiquetar | | | 4,00 | | |
| Encartuchar | | | | | 5,25 |
| Colocar na master | | | | | 2,25 |
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
| **CARGA (s)** | **11,75** | **22,22** | **20,41** | **18,80** | **16,00** |
| **OCUPAÇÃO (takt 30 s)** | **39,2 %** | **74,1 %** | **68,0 %** | **62,7 %** | **53,3 %** |

**Atividades de controle isoladas:**

| Atividade | s/peça |
|---|---|
| Inspeção Pino | 1,083 |
| Inspeção Equiptop | 1,360 |
| Inspeção Caixa (1/25) | 0,367 |
| Inspeção Caixa (1/50) | 2,040 |
| **Inspeção Montagem** | **6,800** |
| Diário de bordo (6 registros) | 6,000 |
| Atualizar quadro | 1,000 |
| **TOTAL DE CONTROLE** | **18,650 s/peça** |

> **As atividades de controle sozinhas representam 18,65 s/peça — 62,2 % do takt de 30 s e 20,9 % de toda a carga do cenário BALANCEADO (2).**
>
> **Esta é a prova numérica de que o MeasurLink é pré-requisito para qualquer redução de quadro:** sem eliminar os 18,65 s de controle, a célula precisa de 89,18 ÷ 30 = **2,97 → 3 operadores no mínimo absoluto**, e os cenários de 3 operadores da planilha (que ignoram o controle) são, na prática, cenários de 4 a 5 operadores.

#### 3.6.7 Por que os cenários de 3 operadores não são executáveis

| Cenário | Carga total | Ocup. máxima | Diagnóstico |
|---|---|---|---|
| CENÁRIO 1 | 72,53 s | **99,5 %** | Zero folga. Qualquer micro-parada gera atraso. |
| CENÁRIO 2 | 72,53 s | **95,2 %** | Folga de 1,34 s por ciclo. |
| CENÁRIO 3 | 72,53 s | **95,2 %** | Idem, com Op3 a 92,9 %. |
| NOVO LAYOUT 3 OP | 71,53 s | **94,6 %** | Folga de 1,50 s. |
| NOVO LAYOUT 3 OP CEN 2 | 71,53 s | **96,4 %** | Folga de 1,00 s. |

**Três motivos de inviabilidade, em ordem de gravidade:**

1. **Nenhum inclui as atividades de controle (18,65 s/pç).** Somando-as, a carga vai a ~90-91 s → **3,25 operadores**, ou seja, **4 operadores**.
2. **Ocupação acima de 94 % não é sustentável** em operação com variabilidade. A prática recomenda teto de 85 %.
3. **O takt de 28 s desses cenários pressupõe 3.086 pç/dia, que o gargalo não entrega** (§3.6.2).

#### 3.6.8 Simulação horária de WIP (abas `Planilha3 (2)` e `CONSOLIDAÇÃO`)

Padrão cíclico identificado, **com repetição a cada 8 horas**:

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

**Eventos de parada registrados na simulação de 25 horas:**

| Evento | Ocorrências | Detalhe |
|---|---|---|
| Embalagem com produção **zero** | **6 horas** (10:00, 11:00, 20:00, 22:00, 02:00, 03:00) | WIP acumulado à frente chega a **249 peças** |
| Equiptop com produção **zero** | **2 horas** (15:00 e 01:00) | WIP de 119 peças represado |
| Montagem com produção **zero** | **4 horas** | WIP de até 258 peças |

**Totais acumulados ao fim do horizonte (aba `Planilha3 (3)`):**

| Etapa | Peças |
|---|---|
| Pino | 38.675 |
| Equiptop | 37.581 |
| Caixa | 36.984 |
| Montagem | 35.892 |
| Embalagem | 35.166 |

**Perda em cascata do pino até a embalagem: 3.509 peças (−9,1 %)** — WIP retido no sistema.

A aba `Planilha3 (3)` registra ainda **capacidade restante negativa** de forma recorrente no **Equiptop (−0,25)** e na **Caixa 1 (−0,14)**, indicando sobrecarga sistemática dessas estações no Método 2.

> **Diagnóstico da simulação:** o WIP **oscila ciclicamente em vez de estabilizar**, e há alternância de *starvation* (falta de peça) e *blocking* (acúmulo) nas mesmas estações. É a assinatura de um sistema **não nivelado**, operando em lote com dois métodos alternados.

#### 3.6.9 Comparativo de produtividade (aba `Planilha1`)

| Medição | Série A | Série B |
|---|---|---|
| 1 | 631 | 2.062 |
| 2 | 1.317 | 2.047 |
| 3 | 1.561 | 2.109 |
| 4 | 1.485 | 1.663 |
| **Média** | **1.248,50** | **1.970,25** |
| **Razão A/B** | **63,37 %** | |

Os valores são compatíveis com **peças produzidas por turno** em dois estados (atual vs. referência), indicando **potencial de +57,8 % de produção** com a mesma estrutura. A razão de **63,4 %** é próxima da eficiência de **69,2 %** medida em E1 (abr/2024), o que **corrobora a consistência entre os dois estudos**.

---

### 3.7 Ferramenta GBO + Yamazumi — **13/06/2025** ⭐ ESTUDO MAIS RECENTE

> **Arquivo:** `Ferramenta GBO + YAMAZUMI - Rev1 ( Manipulação 4 operadores).xlsm`
> **Elaborador:** **David Avila Teixeira** — Departamento de **Engenharia**
> **Data declarada na planilha:** **03/03/2025**
> **Datas do arquivo:** criado em **03/03/2025 00:57**, última edição em **13/06/2025 09:41**
> **Idade:** **1 ano e 4 meses — o dado mais recente da base**
> **Processo:** Montagem MTD · **Produto 335272** · **Método: análise de vídeo**

#### 3.7.1 Parâmetros do estudo

| Parâmetro | Valor |
|---|---|
| Tempo disponível | **1.260 min/dia (21 h)** · 31.500 min/mês |
| Dias úteis | 25 dias/mês |
| **Demanda** | **230.000 peças/mês = 9.200 peças/dia** |
| **Takt Time** | **8,217 s** |
| Capacidade necessária | 561,66 pç/h · 11.794,87 pç/dia |
| Eficiência necessária | **78 %** |
| Tempo necessário | 21h00 |

> ⚠ **Escopo diferente do TD10:** este estudo trata da **montagem da família MTD inteira** (230.000 pç/mês), não da linha TD10 isolada (62.332 pç/mês em E1). São complementares, não contraditórios — mas os números **não podem ser misturados**.

#### 3.7.2 ESTADO ATUAL — 5 postos

| Posto | Operação | Movim. | Tméd (s) | Coef. fadiga | **Tméd ajustado (s)** | Ocupação (takt 8,217 s) |
|---|---|---|---|---|---|---|
| OP1 | Fechamento + Gravação + Pré-montagem | 6 | 6,165 | 4,76 % | **6,473** | 78,8 % |
| OP2 | Aplicação do Guarda-pó | 7 | 6,180 | 4,76 % | **6,489** | 79,0 % |
| OP3 | Embalagem saco plástico | 4 | 3,593 | 4,76 % | **3,772** | 45,9 % |
| **OP4** | **Cartucho** | 7 | 7,464 | 4,76 % | **7,837** | **95,4 %** |
| OP5 | Master | **22** | 5,590 | **13,04 %** | **6,428** | 78,2 % |
| | **TOTAL** | **46** | | | **31,00 s** | |

**Indicadores do estado atual:**

| Indicador | Valor |
|---|---|
| Gargalo declarado | **6,473 s** (OP1) |
| **Lead Time** (soma dos ciclos) | **28,991 s** |
| **Capacidade instalada** | **556,13 pç/h = 11.678,83 pç/dia** |
| Nº de postos teórico (pelo takt) | 3,53 → 4 |
| Nº de postos teórico (pelo gargalo) | 4,48 → **5** |
| **Eficiência** | **88,20 %** |
| Tempo necessário | **16h32min33s** (contra 21 h disponíveis) |

**Decomposição AV / Necessário / Desperdício:**

| Posto | Agrega valor (s) | Necessário (s) | Desperdício (s) | % desperdício |
|---|---|---|---|---|
| OP1 | 0,465 | 4,415 | 1,285 | 20,9 % |
| OP2 | 0,570 | 5,610 | 0,000 | 0 % |
| OP3 | 1,389 | 1,004 | 1,200 | 33,4 % |
| **OP4** | 1,938 | 2,437 | **3,089** | **41,4 %** ❌ |
| OP5 | 0,000 | 4,295 | 1,294 | 23,2 % |
| **TOTAL** | **4,362** | **17,761** | **6,868** | |
| **% do total** | **15,0 %** | **61,3 %** | **23,7 %** | |

> **Apenas 15 % do tempo da montagem agrega valor.** O **OP5 (Master) não tem NENHUMA atividade que agrega valor** — é 100 % manipulação e embalagem.

#### 3.7.3 ESTADO PROPOSTO — 4 postos

**Atividades marcadas como "Manter? Não" (eliminadas):**

| Posto | Atividade eliminada | Tempo ajustado (s) |
|---|---|---|
| OP1 | Esperar para retirar a peça | 0,500 |
| OP4 | Arrumar cartuchos fechados na mesa | 0,600 |
| OP4 | Disponibiliza o cartucho fechado para a próxima operação | 1,289 |
| OP4 | Grampear as abas da parte superior da caixa | 0,059 |
| OP4 | Grampear parte de baixo da caixa | 0,082 |
| OP4 | Guardar o grampeador (2 ocorrências) | 0,102 |
| OP4 | Pegar grampeador e posicionar (2 ocorrências) | 0,107 |
| OP4 | Pegar pincel, abrir e marcar a etiqueta, fechar e guardar | 0,200 |
| | **TOTAL ELIMINADO** | **≈ 2,94 s** |

> **Toda a operação de grampeamento manual foi eliminada**, o que pressupõe seladora automática ou caixa auto-montável. Também foi eliminado o **check com pincel atômico** — que é a **operação 11 do TPO043** (E9). **A eliminação exige revisão formal do trabalho padrão.**

**Novo arranjo (OP4 absorve o posto MASTER):**

| Posto | Operação | Movim. | Tméd (s) | Coef. fadiga | **Tméd ajustado (s)** | Ocupação (takt 8,217 s) |
|---|---|---|---|---|---|---|
| OP1 | Fechamento + Gravação + Pré-montagem | 6 | 5,300 | 2,91 % | **5,459** | 66,4 % |
| OP2 | Aplicação do Guarda-pó | 7 | 5,520 | 2,91 % | **5,686** | 69,2 % |
| OP3 | Embalagem saco plástico | 4 | 3,578 | 4,76 % | **3,757** | **45,7 %** |
| **OP4** | **Cartucho + Master** | 7 | 9,867 | 2,91 % | **10,163** | **123,7 %** ❌ |
| | **TOTAL** | | | | **25,06 s** | |

**Indicadores comparados:**

| Indicador | Atual | **Proposto** | Variação |
|---|---|---|---|
| Gargalo declarado | 6,473 s | **5,459 s** | **−15,7 %** |
| Lead Time | 28,991 s | **24,265 s** | **−16,3 %** |
| Capacidade instalada | 556,13 pç/h | **659,46 pç/h** | **+18,6 %** |
| Capacidade/dia | 11.678,83 pç | **13.848,69 pç** | **+18,6 %** |
| Nº de postos (takt) | 3,53 → 4 | 3,79 → 4 | — |
| **Eficiência** | 88,20 % | **94,64 %** | **+6,44 p.p.** |
| Tempo necessário | 16h32min | **13h57min** | **−2h35min** |
| **Nº real de postos** | **5** | **4** | **−1 operador** |

**Decomposição AV / Necessário / Desperdício:**

| | Atual | Proposto | Variação |
|---|---|---|---|
| Agrega valor | 4,362 s (15,0 %) | 4,242 s (17,3 %) | **+2,3 p.p.** |
| Necessário | 17,761 s (61,3 %) | 16,346 s (66,7 %) | −1,415 s |
| **Desperdício** | **6,868 s (23,7 %)** | **3,677 s (15,0 %)** | **−46,5 %** ✅ |

#### 3.7.4 ⚠ ERRO TÉCNICO NA PROPOSTA — e a correção

> **A proposta de 4 postos declara gargalo de 5,459 s, mas o OP4 (Cartucho + Master) fica com 10,163 s — 23,7 % ACIMA do takt de 8,217 s.**
>
> **A proposta, como está, não é executável:** consolidar Cartucho e Master em um único operador **cria um gargalo pior que o original** (10,163 s contra 7,837 s do OP4 atual). A capacidade real do arranjo proposto seria **3.600 ÷ 10,163 = 354 pç/h**, e não os 659 pç/h declarados — **46 % abaixo do anunciado**.

**Correção recomendada — redistribuição OP4 → OP3:**

| Posto | Proposta original | **Proposta corrigida** | Ocupação corrigida |
|---|---|---|---|
| OP1 | 5,459 s | 5,459 s | 66,4 % |
| OP2 | 5,686 s | 5,686 s | 69,2 % |
| **OP3** | 3,757 s (45,7 % — **4,46 s de folga**) | **≈ 6,26 s** | **76,2 %** ✅ |
| **OP4** | **10,163 s (123,7 %)** ❌ | **≈ 7,66 s** | **93,2 %** ⚠ |

**Candidatas naturais à transferência (atividades de baixo acoplamento do OP4):**

| Atividade | Tempo (s) | Justificativa |
|---|---|---|
| Pegar a etiqueta, descolar e aplicar na caixa | 0,271 | Independente do fluxo do cartucho |
| Colar etiqueta no cartucho | 0,950 | Pode ser feita no posto anterior |
| Imprimir etiquetas | 0,267 | Atividade de preparação |
| Abastecer a caixa com cartuchos | 0,778 | Pode ser compartilhada |
| Recortar/organizar etiquetas | 0,260 | Preparação |
| **Soma transferível** | **≈ 2,53 s** | Leva OP4 a 7,63 s e OP3 a 6,29 s |

> **Com essa correção, ambos ficam abaixo do takt de 8,217 s e o arranjo de 4 postos torna-se viável.** O OP4 a 93,2 % ainda é alto — a alternativa mais robusta é **automatizar a montagem/fechamento da caixa master**, o que também elimina o risco ergonômico do OP5 descrito a seguir.

#### 3.7.5 Achado ergonômico

| Posto | Movimentações | Tempo (s) | **Coef. de fadiga** |
|---|---|---|---|
| OP1 | 6 | 6,165 | 4,76 % |
| OP2 | 7 | 6,180 | 4,76 % |
| OP3 | 4 | 3,593 | 4,76 % |
| OP4 | 7 | 7,464 | 4,76 % |
| **OP5 (Master)** | **22** | 5,590 | **13,04 %** |

> **O posto MASTER concentra 22 das 46 atividades (47,8 %) em apenas 5,59 s de tempo — e tem coeficiente de fadiga 2,7× maior que todos os demais.** É o posto de maior fragmentação e manipulação da linha, com **zero atividades que agregam valor**. É simultaneamente o maior risco ergonômico e o maior alvo de automação.

#### 3.7.6 Concentração de etiquetagem

| Atividade de etiqueta | Tempo ajustado (s) |
|---|---|
| Colar etiqueta no cartucho | 0,950 |
| Imprimir etiquetas | 0,400 |
| Recortar as etiquetas e organizar para aplicar | 0,283 |
| Pegar a etiqueta, descolar e aplicar na caixa | 0,271 |
| Recolher o fim das etiquetas e colocar no lixo | 0,050 |
| **TOTAL** | **1,954 s/peça = 23,8 % do takt** |

> **Cinco atividades distintas apenas para etiquetar.** Um aplicador automático de etiquetas endereça **1,95 s/peça (23,8 % do takt)** — provavelmente o melhor retorno isolado da montagem.

#### 3.7.7 As 46 atividades (tabela integral do estado atual)

| Posto | Atividade | MOP | Classe | Tméd (s) | Freq. | **Tméd ajust. (s)** |
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
| OP5 | Recortar etiquetas e organizar para aplicar | TOM | **DESPERDÍCIO** | 14,17 | 50 | 0,283 |
| OP5 | Imprimir etiquetas | TOM | NECESSÁRIO | 180,0 | 450 | 0,400 |
| | **TOTAL GERAL (46 atividades)** | | | | | **28,991 s** |

*MOP: **TMP** = Trabalho Máquina-Parada · **TOM** = Trabalho Operador-Máquina · **TMO** = Trabalho Manual-Operador.*

---

### 3.8 Trabalho padrão TPO040 e TPO043 — **fev e abr/2024**

#### 3.8.1 TPO040 — PINO / TERMINAL — Torno CNC — **27/02/2024**

> **Arquivo:** `trabalhopadrao/TPO040.pdf` · **PDF gerado em 27/02/2024 15:14** · Idade: 2 anos e 7 meses

| Campo | Conteúdo |
|---|---|
| **Produto** | PINO / TERMINAL |
| **Equipamento** | TORNO CNC |
| **Tempo de ciclo** | **TD10/TD20/TD30 = tempo máquina + 7 s** · TD40 = tempo máquina + 4 s |
| **EPIs** | Luva de corte · luva antivibratória · sapato · protetor auricular · óculos |

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
| | **Subtotal homem** | **14** | |
| 11 | Troca de inserto na frequência estipulada pelo programa CNC | | |
| 12 | Inspeção realizada conforme **PC001** | | |
| 13 | **Peça de setup pintada de VERDE** na região do arraste | 2 | |
| 14 | **Peça de inspeção pintada de AMARELO** na região do arraste | 2 | |
| 15 | Separadores nas caixas quando houver mais de uma OP no trilho | 3 | |
| 16 | **Peça de sucata pintada de VERMELHO** | | |

> **Sistema de gestão visual por cor padronizado e vigente:** VERDE = setup · AMARELO = inspeção · VERMELHO = sucata.

#### 3.8.2 TPO043 — EMBALAGEM GUARDA-PÓ CAIXA DE DIREÇÃO — **01/04/2024**

> **Arquivo:** `trabalhopadrao/TPO043.pdf` (TPO043-01) · **PDF gerado em 03/04/2024 11:33** por Edison Schmitz de Oliveira
> **Controle de revisão declarado no documento:**
> - **Rev. 0 — 13/11/2023** — Elaboração do documento — David Teixeira / Maicon Lemos / José Guedes
> - **Rev. 1 — 01/04/2024** — Inclusão das imagens de referência — David Teixeira / Maicon Lemos / José Guedes
>
> **Idade:** 2 anos e 6 meses · *"Sem validade se impresso"*

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
| 11 | Fechar a caixa master e fazer **check com pincel atômico**, garantindo a etiqueta grande |

**Componentes:** guarda-pó · saco plástico · etiqueta master · etiqueta do saco plástico.

> ⚠ **Conflito com E7 (jun/2025):** a **operação 11** deste padrão vigente ("check com pincel atômico") corresponde exatamente à atividade *"Pegar pincel, abrir e marcar a etiqueta, fechar e guardar novamente"* (3,600 s brutos · 0,200 s/pç), classificada como **DESPERDÍCIO** e **marcada para eliminação** no estudo mais recente. **Eliminar a atividade exige revisar e reaprovar o TPO043 (Rev. 2).**

#### 3.8.3 Documentos de referência citados (ausentes do repositório)

| Documento | Função | Criticidade |
|---|---|---|
| **PC001** | Plano de controle — inspeção do pino (gargalo) | 🔴 Alta |
| **IT 215** | Instrução — abertura de ordem de produção | 🟡 Baixa |
| **IT 147** | Instrução — impressão de etiquetas | 🟡 Baixa |
| **FO021** | Formulário de registro de inspeção em papel — objeto da eliminação pelo MeasurLink | 🟠 Média |

---

## 4. LINHA DO TEMPO E EVOLUÇÃO DOS PARÂMETROS

### 4.1 Cronologia dos estudos

```
2024                                              2025
 │                                                 │
 ├─ FEV ─── TPO040 (27/02) ─ trabalho padrão Pino
 │
 ├─ ABR ─┬─ TPO043 Rev.1 (01/04) ─ embalagem guarda-pó
 │       └─ E1 GBO TERMINAL (17-18/04) ⭐ takt 37,43 s · efic. 69,2 %
 │
 ├─ MAI ─── E2 SHINGO (22/05) ⚠ lead time 14,13 dias
 │
 ├─ JUL ─┬─ E3 PRESSMATIK (01-04/07) ─ ciclo 46,88 → 34,26 s
 │       └─ [criação do modelo GBO Rev06/07 em 11/07]
 │
 ├─ AGO ─── E4 MEASURLINK (06-13/08) ─ R$ 56.419 · R$ 270.284 de ganho
 │
 │                                            MAI ─┬─ E5 Rev06-1 (04/05)
 │                                                 └─ E6 Rev07 (08/05) ⭐
 │                                                     perdas 106,7 %
 │
 │                                            JUN ─── E7 YAMAZUMI (13/06) ⭐⭐
 │                                                     montagem 5 → 4 postos
 ▼                                                 ▼
                                                            HOJE: 07/10/2026
                                                            (1a4m desde o último estudo)
```

### 4.2 Evolução do takt time ao longo dos estudos

| Data | Estudo | Takt (s) | Escopo | Demanda implícita |
|---|---|---|---|---|
| **04/2024** | E1 | **37,43** | TD10 (linha) | 62.332 pç/mês |
| **07/2024** | E3 | **31,50** | Pressmatik (posto) | ≈ 74.100 pç/mês |
| **05/2025** | E6 | **30,00** | Célula TD10 — estado atual e balanceados | ≈ 77.760 pç/mês |
| **05/2025** | E5/E6 | **28,00** | Célula TD10 — cenários futuros | ≈ 83.314 pç/mês |
| **06/2025** | E7 | **8,22** | Montagem família MTD | 230.000 pç/mês |

> **Tendência inequívoca:** o takt do TD10 caiu de **37,43 s (abr/2024) para 28 s (mai/2025)** — uma **redução de 25,2 % em 13 meses**, equivalente a um **aumento de demanda de 33,7 %**. Os estudos sucessivos foram se ajustando a uma demanda crescente.
>
> **Implicação:** a capacidade do gargalo (2.856 pç/dia) **não acompanhou** esse crescimento. Em abr/2024 havia folga teórica de 13,4 %; em mai/2025 há **déficit nominal de 7,4 %**.

### 4.3 Evolução do dimensionamento de operadores

| Data | Estudo | Cenário | Nº operadores | Carga total (s) | Observação |
|---|---|---|---|---|---|
| 04/2024 | E1 | Cálculo por takt | **1,60 → 2** | 59,76 | Linha TD10, base trabalho manual |
| 05/2025 | E6 | Estado atual | **5** | 71,42 | Com Op. Montagem a 136,9 % |
| 05/2025 | E6 | BALANCEADO (2) | **5** | 89,18 | **Único com controle incluído** |
| 05/2025 | E5 | Novo layout | **4** | 69,03 | Sem controle |
| 05/2025 | E6 | Método 1 | **4** | 57,53 | Sem controle |
| 05/2025 | E6 | Cenários 1-3 | **3** | 72,53 | ❌ Sem controle, ocup. 95-99,5 % |
| 06/2025 | E7 | Montagem proposta | **4** (era 5) | 25,06 | ❌ OP4 a 123,7 % |

---

## 5. DIAGNÓSTICO CONSOLIDADO

### 5.1 As 7 perdas estruturais evidenciadas pela base recente

| # | Perda | Magnitude | Estudo | Data | Severidade |
|---|---|---|---|---|---|
| **1** | **Paradas planejadas excedem o tempo de turno** | **28.178 s vs. 26.400 s = 106,7 %** | E6 | 05/2025 | 🔴 CRÍTICA |
| **2** | **79 % do trabalho manual não agrega valor** | 59,76 s: 21,2 % AV · 46,7 % NNAV · 32,1 % D | E1 | 04/2024 | 🔴 CRÍTICA |
| **3** | **Inspeções e registros = 59,2 % das perdas** | 16.700 s/turno (inspeção da montagem sozinha: 7.000 s) | E6 | 05/2025 | 🔴 CRÍTICA |
| **4** | **Gargalo sem capacidade nominal para o takt** | 2.856 pç/dia vs. 3.086 exigidas = **−7,4 %** | E6 | 05/2025 | 🔴 CRÍTICA |
| **5** | **Desbalanceamento extremo da célula** | Op. Montagem a **136,9 %** vs. 4 operadores a 22-29 % | E6 | 05/2025 | 🟠 ALTA |
| **6** | **Montagem: 85 % do tempo não agrega valor** | 15,0 % AV · 61,3 % necessário · 23,7 % desperdício | E7 | 06/2025 | 🟠 ALTA |
| **7** | **Lead time de 14 dias com 0,007 % de VA** ⚠ | 20.347 min · 98,19 % de espera | E2 | 05/2024 | 🟡 A REVALIDAR |

### 5.2 Cadeia causal

```
         INSPEÇÃO MANUAL + REGISTRO EM PAPEL (FO021)
                   13.340 s + 3.360 s = 16.700 s/turno
                                │
                                ▼
          PERDAS DE DISPONIBILIDADE = 106,7 % DO TURNO
                                │
                 ┌──────────────┴──────────────┐
                 ▼                             ▼
     EFICIÊNCIA REAL DE 69,2 %      PADRÃO NÃO EXECUTÁVEL
     (E1, mar-abr/2024)             (inspeções puladas,
                 │                   registros em lote)
                 ▼                             │
   GARGALO EFETIVO = 2.856 × 0,692             │
              = 1.976 pç/dia                   │
                 │                             │
                 ▼                             ▼
   DÉFICIT DE 36 % CONTRA O TAKT        PERDA DE CONTROLE
   DE 28 s (3.086 pç/dia exigidas)      ESTATÍSTICO
                 │                             │
                 └──────────────┬──────────────┘
                                ▼
            376 SUCATAS + 9.425 PEÇAS COM RETRABALHO/DESVIO
                    (E4, base 06/2023 – 06/2024)
                                ▼
                  R$ 103.488 DE FATURAMENTO AFETADO
```

### 5.3 Os três pontos de alavancagem, com base apenas nos dados recentes

| # | Alavanca | Perdas que ataca | Impacto calculado | Estudo de suporte |
|---|---|---|---|---|
| **1** | **MeasurLink no gargalo e depois na linha** | #1, #3, #7 | Perdas de **106,7 % → 75,1 %**; eficiência de **69,2 % → ~85 %**; R$ 270.284 de ganho | E4 (08/2024) + E6 (05/2025) |
| **2** | **Liberar capacidade no gargalo (pino)** | #4 | Fechar o déficit de **230 pç/dia** no takt de 28 s | E6 (05/2025) |
| **3** | **Rebalancear célula e montagem** | #2, #5, #6 | Célula: **5 → 4 operadores reais**; Montagem: **5 → 4 postos (+18,6 % de capacidade)** | E6 + E7 (2025) |

> **Sequência obrigatória: 1 → 2 → 3.** A alavanca 3 é matematicamente impossível antes da 1, porque as atividades de controle (18,65 s/pç) consomem 62,2 % do takt de 30 s e estão incluídas no único cenário realista da base (BALANCEADO 2).

---

## 6. DIVERGÊNCIAS ENTRE OS ESTUDOS RECENTES

Mesmo restringindo a base a 2024-2025, persistem inconsistências que **precisam ser resolvidas antes de decisões de investimento**.

### 6.1 Capacidade do gargalo

| Valor | Estudo | Data |
|---|---|---|
| **119 pç/h** (2.856 pç/dia) | E6 — aba `Planilha4` | 05/2025 |
| **118,8 pç/h** (ciclo de 30,3 s) | E6 — aba `Planilha3 (2)` | 05/2025 |
| **128 pç/h** | E4 — base de cálculo do ganho de capabilidade | 08/2024 |

**Impacto:** o ganho declarado de **R$ 112.640 por máquina** (E4) usa 128 pç/h. Com 119 pç/h, o mesmo cálculo resulta em **R$ 104.720** — **7,0 % menor**. O caso de negócio permanece válido, mas o valor deve ser corrigido.

### 6.2 Tempo de virada (dentro do mesmo arquivo E6)

| Valor | Aba | Diferença |
|---|---|---|
| **3.600 s × 2 = 7.200 s** | `PERDAS DE DISPONIBILIDADE` | — |
| **10.800 s** | `Planilha2` | **+50 %** |

**Impacto:** 3.600 s representam **12,8 % das perdas totais**. Se o valor correto for 10.800 s, a razão de perdas sobe de **106,7 % para 120,3 %**.

### 6.3 Tempo de setup (três valores para o mesmo setup)

| Setup | E1 (04/2024) | E6 — `PERDAS` (05/2025) | E6 — `Planilha2` (05/2025) |
|---|---|---|---|
| **Pino** | 594 s | **720 s** | **1.800 s** |
| **Equiptop** | 1.674 s | **1.758 s** | — |
| **Caixa** | 1.800 s | **1.800 s** | — |

**Impacto:** o setup do pino varia **203 %** entre fontes. Como o pino é o gargalo, essa divergência afeta diretamente o cálculo de capacidade.

### 6.4 Tempo de "Inserir Bucha"

| Valor | Onde | Data |
|---|---|---|
| **8,22 s** | E6 — aba `ESTADO ATUAL` | 05/2025 |
| **8,22 s** | E3 — média da bucha no Cenário 1 | 07/2024 |
| **2,00 s** | E6 — todos os demais cenários | 05/2025 |

**Impacto:** 6,22 s/peça = **22,2 % do takt de 28 s**. É a maior divergência unitária da base. A coincidência entre E3 e o ESTADO ATUAL de E6 sugere que **8,22 s é o valor medido** e **2,00 s é uma meta otimista não validada** — o que tornaria todos os cenários futuros de E6 otimistas em 6,22 s.

### 6.5 Takt time

Cinco valores (37,43 / 31,50 / 30 / 28 / 8,22 s) em cinco estudos. **Não são erros** — refletem escopos e épocas diferentes (§4.2) —, mas **nenhum documento declara explicitamente o escopo e a data-base de seu takt**, o que facilita o uso cruzado indevido.

### 6.6 Quadro-resumo das divergências

| # | Item | Amplitude | Afeta | Prioridade de resolução |
|---|---|---|---|---|
| 1 | Capacidade do gargalo | 119 ↔ 128 pç/h (**+7,6 %**) | Caso de negócio do MeasurLink | 🔴 Alta |
| 2 | Tempo de virada | 7.200 ↔ 10.800 s (**+50 %**) | Razão de perdas (106,7 % ↔ 120,3 %) | 🔴 Alta |
| 3 | Setup do pino | 594 ↔ 1.800 s (**+203 %**) | Capacidade do gargalo | 🔴 Alta |
| 4 | Inserir bucha | 2,00 ↔ 8,22 s (**+311 %**) | Todos os cenários de balanceamento | 🔴 Alta |
| 5 | Takt time | 28 ↔ 37,43 s (TD10) | Dimensionamento de quadro | 🟠 Média |

---

## 7. O QUE FOI DESCARTADO E POR QUÊ

### 7.1 Documentos excluídos da base

| Documento | **Data real** | Idade em 07/10/2026 | Motivo da exclusão |
|---|---|---|---|
| `trabalhopadrao/TPO041.pdf` (Equiptop) | **21/10/2023** | 3 a 0 m | Anterior ao corte |
| `trabalhopadrao/TPO042.pdf` (Cachimbo/Torno) | **21/10/2023** | 3 a 0 m | Anterior ao corte |
| `GBO Montagem.xlsx` | conteúdo **10/03/2023** (re-save 28/09/2026) | 3 a 7 m | Anterior ao corte — ver §7.3 |
| `fluxo macro.xlsx` | **20/12/2022** | 3 a 10 m | Cronograma **vencido** (nov/2023 a nov/2024) |
| `GBO - Laminadoras.xlsx` | **16/12/2022** | 3 a 10 m | Anterior ao corte |
| `Projeto fluxo por familia (piloto celula terminal).xlsx` | **16/11/2022** | 3 a 11 m | Orçamentos e cronograma vencidos |
| `Fluxograma Linha 10.pptx` | **10/11/2022** | 3 a 11 m | Layout possivelmente alterado desde então |
| `lista de materiais.xlsx` | **18/10/2022** | 4 a 0 m | **Preços de 24/09/2022** — defasados |
| `Exemplo de estratificação de set up.xlsx` | **30/08/2022** (dados de 2021) | 4 a 1 m | Dados de **outras máquinas** (extrusoras, PH630, CNC20/21) |
| `Fluxograma do Teste Piloto.pptx` | **21/06/2022** | 4 a 4 m | Anterior ao corte |
| `Troca Rápida de Ferramentas.pptx` | **25/09/2018** | 8 a 0 m | Material de treinamento, sem dados do TD10 |
| `workshop_pps_v1.pdf` | **15/02/2018** (evento 05/02/2018) | 8 a 8 m | Treinamento de PPCP, sem dados do TD10 |
| **`MFV - Terminal de Direção 335074 - Rev. 00.xls`** | **21/03/2011** ⚠ | **15 a 7 m** | **Ver §7.2 — achado crítico** |
| **`Antropometria_PostosdeTrabalho[1].pdf`** | **16/08/2005** ⚠ | **21 a 2 m** | **Ver §7.2** |

### 7.2 Dois achados importantes sobre a idade real de documentos em uso

#### ⚠ Achado 1 — O MFV do Terminal de Direção é de **2011**

| Metadado | Valor |
|---|---|
| Arquivo | `MFV - Terminal de Direção 335074 - Rev. 00.xls` |
| **Criado em** | **07/02/2011 14:45** |
| **Último salvamento** | **21/03/2011 14:10** |
| Autor | "Vaio" |
| Último editor | "Rolim" |
| Revisão | 00 |

**Por que isso importa:** este MFV contém os números frequentemente citados como diagnóstico do fluxo — lead time de **334,13 h (13,92 dias)**, **2,13 % de valor agregado**, **870 m** de movimentação, **221,17 h** de espera por processamento. **Todos esses números têm mais de 15 anos** e descrevem um arranjo fabril, um mix e uma estrutura de fornecedores que muito provavelmente não existem mais.

**Elementos do MFV de 2011 que certamente mudaram:** o próprio projeto de fluxo por família (2022) previa reconfigurar a linha, absorver as máquinas do TD20 e instalar trilhos roletados; o MeasurLink (2024) altera o bloco de inspeção; os estudos de 2025 adotam takt 25 % menor.

> **Recomendação:** o MFV deve ser **refeito integralmente** (Rev. 01) antes de qualquer decisão de layout, lote ou buffer. Nenhum número dele foi usado neste relatório.

#### ⚠ Achado 2 — A tabela antropométrica é de **2005**

| Metadado | Valor |
|---|---|
| Arquivo | `Antropometria_PostosdeTrabalho[1].pdf` |
| **Criado em** | **16/08/2005 13:38** |
| Gerador | PDF-XChange 3.30.0059 (Windows XP) |

A tabela traz percentis 5 % e 95 % por sexo para 10 medidas corporais e critérios de projeto de posto (sentado e em pé). **São dados de 21 anos atrás.** Tabelas antropométricas da população brasileira foram atualizadas desde então, e a norma de referência para postos de trabalho (NR-17) teve revisão relevante publicada em 2021-2022.

> **Recomendação:** substituir por tabela antropométrica atualizada e pela redação vigente da NR-17 antes de projetar os novos postos — especialmente considerando o risco ergonômico do posto MASTER identificado em E7 (coeficiente de fadiga de 13,04 %).

### 7.3 Caso especial — `GBO Montagem.xlsx`

| Metadado | Valor |
|---|---|
| **Criado em** | **10/03/2023 10:37** — Matheus de Conto Rodrigues |
| **Modificado em** | **28/09/2026 19:23** — **Fabio Antonio Dalla Vecchia** |
| Datas internas no conteúdo | **Nenhuma** |
| Upload ao GitHub | 07/10/2026 (9 dias após a modificação) |

**Decisão: descartado**, com ressalva. A modificação de 28/09/2026 ocorreu 9 dias antes do upload de todos os arquivos ao repositório, por quem fez o upload — padrão compatível com um simples **re-save durante a preparação do pacote**, não com recoleta de dados. Não há marca de revisão, data interna ou alteração estrutural que indique atualização de conteúdo.

**O que este arquivo contém** (e que fica de fora deste relatório): tempos médios de 11 operações de montagem em 10 postos, com 3 a 12 cronometragens cada — incluindo um gargalo de **12,98 s** na "Colocação de Abraçadeira (2)" com variabilidade de 163 %.

> **Ação necessária (§9):** confirmar com Fabio Antonio Dalla Vecchia se houve atualização de conteúdo em set/2026. **Se houve, este passa a ser o estudo mais recente da base** e o relatório deve ser revisado. Como o estudo E7 (jun/2025) cobre a mesma área (montagem) com método mais robusto (46 atividades, análise de vídeo, coeficiente de fadiga), a exclusão tem baixo impacto no diagnóstico.

### 7.4 Impacto da exclusão no diagnóstico

| Tema | Como era tratado com a base completa | Como fica com a base recente |
|---|---|---|
| **Lead time** | 13,92 dias (MFV 2011) + 14,13 dias (Shingo 2024) apresentados como confirmação mútua | **Apenas 14,13 dias (Shingo 2024), com confiabilidade rebaixada.** A "confirmação mútua" era ilusória: o Shingo pode ter herdado os números do MFV de 2011. |
| **% de valor agregado** | 2,13 % (MFV) e 0,007 % (Shingo) | **Apenas 0,007 % (Shingo), a revalidar** |
| **Movimentação de 870 m** | Citado como dado atual | **Removido** — dado de 2011 |
| **Investimento em trilhos/fluxo** | R$ 20.810,27 em OCs aprovadas | **Removido** — orçamentos de 2022, provavelmente já executados ou defasados |
| **Setup / TRF** | Plano de ação com 25 itens e 645 min/mês de ganho | **Removido** — dados de 2021 de outras máquinas. Resta apenas o valor dos setups em E1 e E6. |
| **Ergonomia** | Critérios antropométricos aplicados ao projeto de posto | **Removido** — tabela de 2005. Resta o coeficiente de fadiga de E7. |
| **Gargalo da montagem (12,98 s)** | Identificado via GBO Montagem | **Removido** — substituído pela análise de E7 (OP4 a 7,84 s / 95,4 %) |

> **Conclusão da §7:** restringir a base **fortaleceu** o diagnóstico em vez de enfraquecê-lo. Os quatro achados críticos (perdas de 106,7 %, 79 % de trabalho sem valor, inspeções como 59,2 % das perdas, gargalo sem capacidade) são **todos sustentados exclusivamente por estudos de 2024-2025**. O que se perdeu foram justamente os números cuja idade os tornava indefensáveis.

---

## 8. PLANO DE AÇÃO

### FASE 0 — Resolver as divergências e revalidar (0 a 30 dias) · Custo ≈ 0

| Ação | Base | Entregável |
|---|---|---|
| Definir valor único para a **capacidade do gargalo** (119 vs. 128 pç/h) | §6.1 | Parâmetro oficial |
| Definir valor único para o **tempo de virada** (7.200 vs. 10.800 s) | §6.2 | Razão de perdas corrigida |
| Definir valor único para o **setup do pino** (594 / 720 / 1.800 s) | §6.3 | Capacidade corrigida |
| **Cronometrar "Inserir Bucha"** e decidir entre 2,00 s e 8,22 s | §6.4 | Todos os cenários corrigidos |
| Declarar **escopo e data-base do takt** em cada estudo | §6.5 | Rastreabilidade |
| Confirmar se `GBO Montagem.xlsx` foi atualizado em set/2026 | §7.3 | Inclusão ou exclusão definitiva |
| Consolidar tudo em **GBO TD10 Rev08**, versão única, com data e autor no cabeçalho | — | **Modelo oficial** |

### FASE 1 — MeasurLink (30 a 135 dias) · R$ 56.419,16

| Ação | Prazo | Base |
|---|---|---|
| Executar o **piloto gratuito de 45 dias** da Mitutoyo | Imediato | E4 |
| **Revalidar a especificação técnica** (SQL Server 2014/2016/2017 e Windows 8/10 estão em fim de suporte) | Antes do CAPEX | E4 §3.4.4 |
| Corrigir o caso de negócio com 119 pç/h (R$ 112.640 → R$ 104.720) | Antes do CAPEX | §6.1 |
| Liberar CAPEX | — | — |
| **Fase 1 — máquina gargalo (pino)** | **15 dias** após CAPEX | E4 |
| Digitalizar diário de bordo e quadro (3.360 s/turno) | Em paralelo | E6 |
| Implantar alerta e bloqueio por fora de tolerância | Fase 1 | E4 |
| **Fase 2 — linha TD10 completa** | **90 dias** após CAPEX | E4 |
| **Meta: perdas de 28.178 s → ~17.500 s · razão de 106,7 % → 66,3 % · eficiência de 69,2 % → ~85 %** | | |

### FASE 2 — Liberar capacidade no gargalo (60 a 150 dias) · Custo baixo

| Ação | Ganho estimado | Base |
|---|---|---|
| **SMED nos 3 setups** (4.278 s/turno): filmar, separar interno/externo, converter | **~2.139 s/turno** (−7,6 % das perdas) | E6 |
| Eliminar **"Marcar peça com marcador industrial"** (4,00 s/pç, classe D) via marcação a laser ou poka-yoke | 4,00 s/pç | E1 |
| Reduzir **"Tempo de deslocamento"** (10,00 s/pç, classe D — a maior atividade isolada) via arranjo de posto | até 10,00 s/pç | E1 |
| Atacar as **viradas** (7.200 s/turno, 25,6 % das perdas) por nivelamento de sequenciamento | até 3.600 s/turno | E6 |
| **Meta: fechar o déficit de 230 pç/dia do takt de 28 s** | | |

### FASE 3 — Rebalancear a célula (135 a 180 dias) · Custo ≈ 0

| Ação | Base |
|---|---|
| **Recalcular o GBO sem as atividades de controle eliminadas pelo MeasurLink** (base: 18,65 s/pç) | E6 §3.6.6 |
| Partir do **BALANCEADO (2)** — único cenário com controle incluído, ocupação máxima de 74,1 % | E6 |
| Com ~12 s/pç de controle eliminados, a carga cai de 89,18 s para ~77 s → **2,57 → 3 operadores viáveis com folga** | Derivado |
| **Não adotar os CENÁRIOS 1-3 como estão** — ocupação de 95 a 99,5 % sem contar o controle | §3.6.7 |
| Corrigir o **ESTADO ATUAL**: o Op. Montagem está a 136,9 % enquanto quatro colegas estão abaixo de 29 % | §3.6.5 |

### FASE 4 — Rebalancear a montagem (150 a 200 dias) · Custo ≈ 0 a baixo

| Ação | Base |
|---|---|
| **Corrigir a proposta de 4 postos:** transferir ~2,53 s do OP4 (10,163 s) para o OP3 (3,757 s, com 4,46 s de folga) | §3.7.4 |
| Validar que OP3 ≈ 6,26 s e OP4 ≈ 7,66 s, ambos abaixo do takt de 8,217 s | §3.7.4 |
| Avaliar **aplicador automático de etiquetas** — 5 atividades, **1,954 s/pç = 23,8 % do takt** | §3.7.6 |
| Avaliar **automação do fechamento da caixa master** — elimina o risco ergonômico do OP5 (fadiga de 13,04 %, 22 movimentações, zero AV) | §3.7.5 |
| **Revisar o TPO043 (Rev. 2)** para remover o check com pincel atômico | §3.8.2 |
| **Meta: 5 → 4 postos · capacidade de 556 → 659 pç/h (+18,6 %) · desperdício de 23,7 % → 15,0 %** | E7 |

### FASE 5 — Pressmatik e sustentação (contínuo) · Custo ≈ 0

| Ação | Base |
|---|---|
| **Padronizar o elemento "Caixinha"** da Pressmatik (12,22 s, variação de 105 % entre cenários) para fechar o gap de **2,76 s** contra o takt de 31,5 s | E3 |
| Ampliar a amostra das cronoanálises de 6 para ≥ 10 ciclos (Cenários 3 e 5 da Pressmatik) | §9 |
| **Refazer o MFV (Rev. 01)** — o vigente é de 2011 | §7.2 |
| **Atualizar a referência antropométrica** e aplicar a NR-17 vigente | §7.2 |
| Avaliação de risco ergonômico formal do posto MASTER | E7 |
| Replicar para **TD20, TD30, TD40** (R$ 124.257,48 restantes na família Terminal) | E4 |

### 8.1 Resumo financeiro (apenas valores de estudos recentes)

| Fase | Investimento | Retorno quantificado | Prazo |
|---|---|---|---|
| 0 — Divergências | ≈ 0 | Habilitador | 30 d |
| **1 — MeasurLink** | **R$ 56.419,16** | **R$ 107.770 pontual + R$ 161.832 risco evitado + R$ 681,72/mês** | 135 d |
| 2 — Capacidade do gargalo | Baixo (interno) | ~2.139 s/turno + até 14 s/pç de desperdício | 150 d |
| 3 — Rebalanceamento da célula | ≈ 0 | De 5 para 3 operadores por turno | 180 d |
| 4 — Rebalanceamento da montagem | ≈ 0 a baixo | 1 posto + 18,6 % de capacidade | 200 d |
| 5 — Pressmatik e sustentação | ≈ 0 | Fechamento do takt | Contínuo |
| **TOTAL** | **R$ 56.419,16** | **> R$ 270.000 + redução de quadro** | ~7 meses |

> **Importante:** não foi incluído o investimento de R$ 20.810,27 do projeto de fluxo por família porque suas ordens de compra são de **2022** e estão fora do corte — não há evidência na base recente sobre seu status de execução.

---

## 9. LACUNAS E REVALIDAÇÕES NECESSÁRIAS

### 9.1 Revalidações prioritárias

| # | Item | Por quê | Prioridade |
|---|---|---|---|
| 1 | **Demanda e takt atuais** | O dado mais recente é de mai/2025 (takt 28 s). Em 16 meses a demanda pode ter mudado novamente — a tendência histórica é de crescimento de ~25 % ao ano | 🔴 |
| 2 | **Eficiência atual** | Os 69,2 % são de **março/abril de 2024** — 2,5 anos atrás | 🔴 |
| 3 | **Lead time (E2)** | Pode ter sido herdado da versão de 2022; é o único número da base sem rastreabilidade de coleta | 🔴 |
| 4 | **Status do CAPEX do MeasurLink** | O projeto é de ago/2024. Não há informação sobre liberação, execução ou do piloto de 45 dias | 🔴 |
| 5 | **Especificação técnica do MeasurLink** | SQL Server 2014/2016/2017 e Windows 8/10 estão em fim de suporte em 2026 | 🔴 |
| 6 | **IROG real do gargalo** | Nenhum estudo da base recente mede disponibilidade × performance × qualidade do pino | 🟠 |
| 7 | **`GBO Montagem.xlsx`** | Confirmar se a modificação de 28/09/2026 alterou conteúdo | 🟠 |
| 8 | **Layout físico vigente** | Nenhum documento recente registra o arranjo atual | 🟠 |

### 9.2 Documentos ausentes do repositório mas citados pelos estudos recentes

| Documento | Citado em | Função | Criticidade |
|---|---|---|---|
| **PC001** | TPO040 (E8) | Plano de controle do pino — **o gargalo** | 🔴 Alta |
| **FO021** | MeasurLink (E4) | Formulário de inspeção em papel — objeto da eliminação | 🟠 Média |
| **IT 215** | TPO043 (E9) | Abertura de ordem de produção | 🟡 Baixa |
| **IT 147** | TPO043 (E9) | Impressão de etiquetas | 🟡 Baixa |
| **Trabalho padrão do Equiptop** | — | O TPO041 existe mas é de out/2023, fora do corte | 🟠 Média |
| **MFV atualizado** | — | O vigente é de 2011 | 🔴 Alta |

### 9.3 Limitações metodológicas dos estudos recentes

| # | Limitação | Estudo | Consequência |
|---|---|---|---|
| 1 | **Amostras pequenas:** 6 ciclos nos Cenários 3 e 5 | E3 | O cenário vencedor (34,26 s) tem a menor amostra. Mínimo recomendado: 10 ciclos. |
| 2 | **Ritmo não avaliado:** coluna "Ritmo" uniformemente igual a 1,00 em todas as 46 atividades | E7 | Sem avaliação de ritmo/esforço, os tempos **não constituem tempo padrão formal** |
| 3 | **Coeficiente de fadiga aparentemente arbitrado:** 4,76 % para todos, exceto MASTER (13,04 %) | E7 | Não há referência à tabela de fadiga utilizada |
| 4 | **Rateio de setup sobre lote fixo de 450 peças** | E1 | Se o lote real variar, todos os tempos/peça mudam proporcionalmente |
| 5 | **Cenários de 3 e 4 operadores sem atividades de controle** | E5, E6 | Tornam-se inexequíveis — ver §3.6.7 |
| 6 | **Gargalo da proposta acima do takt** | E7 | A proposta de 4 postos não é executável sem correção — ver §3.7.4 |
| 7 | **Duas cópias byte-idênticas do mesmo arquivo** | E6 | Risco de edição divergente futura. MD5 `0303913a41a23d4007bc15ff4d509952` |
| 8 | **Ausência de cabeçalho com data e autor** nas planilhas | E5, E6 | As datas só foram recuperáveis via metadados do arquivo |

### 9.4 Higiene do repositório

| Item | Recomendação |
|---|---|
| `!!Cópia de Cópia de GBO - TD10 - Rev07.xlsx` | **Excluir** — duplicata exata |
| `Pressmatik/~$Tempos Pressmatik.xlsx` | **Excluir** — arquivo temporário de lock do Excel |
| `Pressmatik/Thumbs.db` | **Excluir** e adicionar ao `.gitignore` |
| Nomes como "Cópia de Cópia de…" e prefixo "!!" | Adotar convenção `GBO_TD10_RevXX_AAAA-MM-DD_autor.xlsx` |
| Abas `Planilha1`, `Planilha2`, `Planilha3 (2)`, `Planilha4` | Renomear com nomes significativos |
| Datas serializadas como `1900-01-01 HH:MM` nas simulações | Formatar como hora, não data-hora |
| Ausência de cabeçalho de identificação nas planilhas | Incluir data, autor, revisão e escopo em todas |

---

## 10. ANEXOS

### Anexo A — Matriz completa de atividades por cenário (E6, Rev07, 08/05/2025)

| Atividade | Estado Atual | Balanceado | Balanceado 2 | Método 1 | Método 2 | 3 OP Cen 2 | Cen 3 OP | Cenário 1 | Cenário 2 | Cenário 3 |
|---|---|---|---|---|---|---|---|---|---|---|
| Abastecimento Pino | 7,00 | 7,00 | 7,00 | 6,00 | 6,00 | 6,00 | 6,00 | 7,00 | 7,00 | 7,00 |
| Abastecimento Equiptop | 6,67 | 12,00 | 12,00 | 12,00 | 12,00 | 12,00 | 12,00 | 10,00 | 10,00 | 10,00 |
| Abastecimento Usinagem Caixa | 7,00 | 7,00 | 7,00 | 5,50 | 11,00 | 11,00 | 11,00 | 14,00 | 14,00 | 14,00 |
| Abastecimento Laminação | — | — | — | 0 | 0 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 |
| Laminação Rosca | 4,00 | 4,00 | 4,00 | — | — | — | — | — | — | — |
| Laminação Esfera | 4,00 | 4,00 | 4,00 | 0 | 0 | 0 | 0 | — | — | — |
| **Inserir Bucha** | **8,22** | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 |
| Adicionar Graxa | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 |
| Abastecer Pressmatik | 4,00 | 4,00 | 4,00 | 6,00 | 6,00 | 6,00 | 6,00 | 5,00 | 5,00 | 5,00 |
| Inserir Porca | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 | 4,86 |
| Peça no saco plástico | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 |
| Selar o saco plástico | 4,50 | 4,50 | 4,50 | 0 | 0 | 4,50 | 4,50 | 4,50 | 4,50 | 4,50 |
| Abrir o cartucho | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 | 2,00 |
| Etiquetar | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 | 4,00 |
| Encartuchar a peça | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 | 5,25 |
| Colocar a peça na master | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 | 2,25 |
| Grampear a caixa | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 | 1,67 |
| **Subtotal operação** | **71,42** | **70,53** | **70,53** | **57,53** | **63,03** | **71,53** | **71,53** | **72,53** | **72,53** | **72,53** |
| Atividades de controle | — | **18,65** | **18,65** | — | — | — | — | — | — | — |
| **CARGA TOTAL** | **71,42** | **89,18** | **89,18** | **57,53** | **63,03** | **71,53** | **71,53** | **72,53** | **72,53** | **72,53** |
| Nº de operadores | 5 | 5 | 5 | 4 | 4 | 3 | 3 | 3 | 3 | 3 |
| Takt (s) | 30 | 30 | 30 | 28 | 28 | 28 | 28 | 28 | 28 | 28 |
| **Ocupação máxima** | **136,9 %** | 85,5 % | **74,1 %** | 69,6 % | 85,8 % | 96,4 % | 94,6 % | 99,5 % | 95,2 % | 95,2 % |

### Anexo B — Simulação horária completa de WIP (E6, aba `Planilha3 (2)`)

| Hora | Prod. Pino | WIP a/Equiptop | Prod. Equiptop | Prod. Caixa 1 | Prod. Caixa 2 | WIP a/Caixa | Prod. Montagem | WIP a/Montagem | Prod. Embalagem | WIP a/Embalagem |
|---|---|---|---|---|---|---|---|---|---|---|
| 06:00 | 119 | 0 | 119 | 103 | 0 | 16 | 103 | 0 | 103 | 0 |
| 07:00 | 119 | 0 | 119 | 103 | 0 | 32 | 103 | 0 | 103 | 0 |
| 08:00 | 119 | 0 | 119 | 103 | 0 | 48 | 103 | 0 | 103 | 0 |
| 09:00 | 119 | 0 | 119 | 103 | 0 | 64 | 103 | 0 | 103 | 0 |
| 10:00 | 119 | 0 | 119 | 103 | 0 | 80 | 103 | 0 | **0** | 103 |
| 11:00 | 119 | 0 | 119 | 103 | 0 | 96 | 103 | 0 | **0** | 206 |
| 12:00 | 119 | 0 | 119 | 103 | 0 | 112 | **0** | 103 | 188 | 18 |
| 13:00 | 119 | 0 | 119 | 103 | 103 | 25 | 125 | 184 | 143 | 0 |
| 14:00 | 119 | 0 | 119 | 103 | 41 | 0 | 125 | 203 | 125 | 0 |
| 15:00 | 119 | 119 | **0** | **0** | 0 | 0 | 203 | 0 | 188 | 15 |
| 16:00 | 119 | 92 | 146 | 103 | 0 | 43 | 103 | 0 | 118 | 0 |
| 17:00 | 119 | 65 | 146 | 103 | 0 | 86 | 103 | 0 | 103 | 0 |
| 18:00 | 119 | 38 | 146 | 103 | 103 | 26 | 125 | 81 | 125 | 0 |
| 19:00 | 119 | 11 | 146 | 103 | 69 | 0 | 125 | 128 | 125 | 0 |
| 20:00 | 119 | 0 | 130 | 103 | 0 | 27 | 225 | 6 | **0** | **225** |
| 21:00 | 119 | 0 | 119 | 103 | 0 | 43 | **0** | 109 | 188 | 37 |
| 22:00 | 119 | 0 | 119 | 103 | 0 | 59 | 212 | 0 | **0** | **249** |
| 23:00 | 119 | 0 | 119 | 103 | 0 | 75 | 103 | 0 | 188 | 164 |
| 00:00 | 119 | 0 | 119 | 103 | 91 | 0 | 125 | 69 | 188 | 101 |
| 01:00 | 119 | 119 | **0** | **0** | 0 | 0 | 69 | 0 | 170 | 0 |
| 02:00 | 119 | 92 | 146 | 103 | 0 | 43 | 103 | 0 | **0** | 103 |
| 03:00 | 119 | 65 | 146 | 103 | 0 | 86 | 103 | 0 | **0** | 206 |
| 04:00 | 119 | 38 | 146 | 103 | 0 | 129 | **0** | 103 | 188 | 18 |
| 05:00 | 119 | 11 | 146 | 103 | 103 | 69 | 125 | 184 | 143 | 0 |
| 06:00 | 119 | 0 | 130 | 103 | 96 | 0 | 125 | **258** | 125 | 0 |

### Anexo C — Fontes e rastreabilidade

| Código | Arquivo | Data do estudo | Hash/identificação |
|---|---|---|---|
| E1 | `GBO TERMINAL.xlsx` | 17-18/04/2024 | aba `TD10` |
| E2 | `SHINGO - AV NAV.xlsx` | 22/05/2024 (criado 07/04/2022) | aba `SHINGO - F3` |
| E3 | `Pressmatik/Tempos Pressmatik.xlsx` | 01-04/07/2024 | abas `CENÁRIO 1/3/4/5`, `COMPARAÇÃO`, `MASTER` |
| E4 | `01 - PROJETO DE CAPABILIDADE TD10( Measure Link ) - atualizado 06.08.24.pptx` | 06-13/08/2024 | 10 slides |
| E5 | `GBO - TD10 - Rev06-1 - ESTUDO DE VIRADAS - DIA A DIA.xlsx` | 04/05/2025 | abas `NOVO LAYOUT`, `NOVO LAYOUT (2)` |
| E6 | `Cópia de Cópia de GBO - TD10 - Rev07.xlsx` | 08/05/2025 | MD5 `0303913a41a23d4007bc15ff4d509952` · 18 abas |
| E7 | `Ferramenta GBO + YAMAZUMI - Rev1 ( Manipulação 4 operadores).xlsm` | 03/03/2025 → 13/06/2025 | 7 abas |
| E8 | `trabalhopadrao/TPO040.pdf` | 27/02/2024 | 1 página |
| E9 | `trabalhopadrao/TPO043.pdf` | Rev.1 01/04/2024 | 2 páginas |

**Método de datação:** metadados internos `docProps/core.xml` (OOXML), metadados `/CreationDate` e `/ModDate` (PDF) e `SummaryInformation` (OLE/`.xls`), cruzados com datas declaradas no conteúdo dos documentos.

---

**FIM DO RELATÓRIO**

*Relatório emitido em 07/10/2026 com base exclusiva em 9 estudos realizados entre 27/02/2024 e 13/06/2025. Treze documentos de 2005 a 2023 foram deliberadamente excluídos e estão listados com suas datas na §7. Todas as divergências remanescentes entre os estudos utilizados estão registradas na §6 e devem ser resolvidas antes da execução do plano de ação.*
