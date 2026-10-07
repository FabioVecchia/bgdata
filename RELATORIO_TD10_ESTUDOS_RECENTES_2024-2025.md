# TD10 — TERMINAL DE DIREÇÃO
### Diagnóstico e plano de ação com base nos estudos de **abr/2024 a jun/2025**

`Emissão 07/10/2026` · `9 estudos usados (datados na §2)` · `13 documentos de 2005–2023 descartados` · `Dado mais recente: 13/06/2025`

---

## 1. O PLACAR

| | Indicador | Valor | Fonte · data |
|---|---|---|---|
| ⏱ | **Takt TD10** | 37,43 s (abr/24) → **28 s** (mai/25) — **−25 % em 13 meses** | E1 · E6 |
| 🧱 | **Gargalo (usinagem do pino)** | 30,3 s · 119 pç/h · **2.856 pç/dia** | E6 · 05/2025 |
| ❌ | **Demanda no takt de 28 s** | 3.086 pç/dia → **déficit de 230 pç/dia (−7,4 %)** | E6 · 05/2025 |
| 🔴 | **Paradas planejadas** | **28.178 s contra 26.400 s de turno = 106,7 %** | E6 · 05/2025 |
| 📉 | **Eficiência medida** | **69,2 %** (campo, mar-abr/2024) | E1 · 04/2024 |
| 🧮 | **Trabalho manual** | 59,76 s/pç — **21,2 % AV · 46,7 % NNAV · 32,1 % desperdício** | E1 · 04/2024 |
| ⚖ | **Desbalanceamento da célula** | Op. Montagem a **136,9 %**, os outros 4 entre 22 % e 29 % | E6 · 05/2025 |
| 🏭 | **Montagem MTD (takt 8,22 s)** | 15 % AV · 23,7 % desperdício · 5 → 4 postos (+18,6 %) | E7 · 06/2025 |
| 💰 | **MeasurLink** | **R$ 56.419,16** de investimento · **R$ 270.283,72** de ganho | E4 · 08/2024 |

### O veredito em seis frases

| # | Conclusão | Evidência |
|---|---|---|
| **1** | **A linha não cabe no turno.** Executando inspeções, viradas, setups e registros conforme a norma, as paradas somam 106,7 % do tempo disponível — não sobra um segundo para produzir. | E6 · 05/2025 |
| **2** | **79 % do esforço humano não agrega valor.** Só 12,67 s dos 59,76 s constroem valor; **8 atividades concentram 63,4 %** do tempo. | E1 · 04/2024 |
| **3** | **O gargalo não suporta o takt de 2025.** 2.856 pç/dia contra 3.086 exigidas — déficit **mesmo a 100 % de eficiência**. Com os 69,2 % reais, cai para 1.976 pç/dia (−36 %). | E6 · 05/2025 |
| **4** | **Os cenários de 3 operadores são inexequíveis.** Carga de 71,5–72,5 s, ocupação de **94,6 % a 99,5 %**, e **nenhum inclui as atividades de controle (18,65 s/pç)**. | E6 · 05/2025 |
| **5** | **A proposta de 4 postos da montagem está errada.** O OP4 consolidado fica em **10,16 s contra takt de 8,22 s (123,7 %)** — a proposta só muda o gargalo de lugar. Correção na §4.7. | E7 · 06/2025 |
| **6** | **O MeasurLink é o primeiro passo, e se paga.** Ataca **59,2 % das perdas** (inspeções + registros) com ROI de +91 % já no ganho pontual. | E4 · 08/2024 |

### A cadeia causal

```
   INSPEÇÃO MANUAL + REGISTRO EM PAPEL (FO021) ....... 16.700 s/turno
                         │
                         ▼
   PARADAS = 106,7 % DO TURNO ──────────► PADRÃO NÃO EXECUTÁVEL
                         │                (inspeção pulada, registro em lote)
                         ▼                          │
   EFICIÊNCIA REAL 69,2 %                           ▼
                         │                 PERDA DE CONTROLE ESTATÍSTICO
                         ▼                          │
   GARGALO EFETIVO 1.976 pç/dia                     ▼
   (−36 % contra o takt de 28 s)      376 SUCATAS + 9.425 PEÇAS COM DESVIO
                         │                 R$ 103.488 de faturamento afetado
                         └──────────────┬───────────┘
                                        ▼
            REDUZIR QUADRO OU REBALANCEAR ANTES DE RESOLVER A INSPEÇÃO
                       É MATEMATICAMENTE IMPOSSÍVEL
```

---

## 2. A BASE DE DADOS

Datas obtidas dos **metadados internos** (`docProps/core.xml`, `/CreationDate` do PDF, `SummaryInformation` do `.xls`), cruzadas com as datas declaradas no conteúdo. Corte adotado: **01/01/2024** — não há documento entre 21/10/2023 e 27/02/2024, logo o corte é limpo.

| Cód. | Estudo | **Data de realização** | Autor | O que traz |
|---|---|---|---|---|
| **E1** | `GBO TERMINAL.xlsx` | **17–18/04/2024** (campo: mar-abr/24) | Alexandre Kichler Martins | 34 eventos cronometrados, takt, eficiência |
| **E2** ⚠ | `SHINGO - AV NAV.xlsx` | criado 07/04/2022 → **atualizado 22/05/2024** | Alexandre Kichler Martins | Lead time e % de VA — **confiabilidade rebaixada** |
| **E3** | `Tempos Pressmatik.xlsx` | **01–04/07/2024** | Laiza Borges da Silva | 4 cenários cronometrados da Pressmatik |
| **E4** | `PROJETO DE CAPABILIDADE TD10 (MeasurLink).pptx` | **06–13/08/2024** (base 06/23–06/24) | D. D. Antunes · P. Frosi | Investimento, ganhos, fases, Projeto F4 |
| **E5** | `GBO TD10 Rev06-1 — Estudo de Viradas.xlsx` | **04/05/2025** | Matheus de Conto Rodrigues | Revisão anterior do modelo |
| **E6** ⭐ | `GBO TD10 Rev07.xlsx` | **08/05/2025** | Matheus de Conto Rodrigues | **Modelo vigente**: capacidade, WIP, 10 cenários, perdas |
| **E7** ⭐ | `Ferramenta GBO + YAMAZUMI Rev1.xlsm` | declarado 03/03/2025 → **salvo 13/06/2025** | David Avila Teixeira | **O mais recente**: 46 atividades da montagem |
| **E8** | `trabalhopadrao/TPO040.pdf` | **27/02/2024** | — | Trabalho padrão Pino / Torno CNC |
| **E9** | `trabalhopadrao/TPO043.pdf` | Rev. 1 — **01/04/2024** | D. Teixeira · M. Lemos · J. Guedes | Trabalho padrão Embalagem guarda-pó |

> ⚠ **E2** foi criado em 2022 e apenas re-salvo em 2024. Não há evidência de recoleta — é o único número da base que **não deve embasar decisão de investimento sem revalidação**.

### O que ficou de fora (e dois achados que isso revelou)

13 documentos de **2005 a 2023**: TPO041/TPO042 (out/23), `GBO Montagem.xlsx` (conteúdo mar/23), `fluxo macro`, `GBO Laminadoras`, `Projeto fluxo por família`, `Fluxograma Linha 10`, `lista de materiais` (preços de set/22), `estratificação de set up` (dados de 2021, outras máquinas), `Fluxograma do Teste Piloto`, `Troca Rápida de Ferramentas` (2018), `workshop_pps` (2018) — todos anteriores ao corte ou sem dados do TD10.

| ⚠ Achado | Impacto |
|---|---|
| **O MFV `Terminal de Direção 335074` é de 21/03/2011** (autor "Vaio", editor "Rolim") | Lead time de 13,92 dias, 2,13 % de VA e 870 m de movimentação **têm 15 anos e foram removidos**. A "confirmação mútua" com o Shingo era ilusória — o Shingo pode ter herdado os valores. **Refazer o MFV (Rev. 01).** |
| **A tabela antropométrica é de 16/08/2005** | 21 anos; a NR-17 teve revisão relevante em 2021-22. **Substituir antes de projetar postos** — sobretudo com o risco ergonômico do posto MASTER (§4.7). |
| **`GBO Montagem.xlsx`: conteúdo de 10/03/2023, re-save em 28/09/2026** por Fabio A. Dalla Vecchia, 9 dias antes do upload | Descartado como re-save de preparação. **Confirmar**: se houve recoleta, passa a ser o estudo mais recente. Impacto baixo — E7 cobre a mesma área com método mais robusto. |

> Restringir a base **fortaleceu** o diagnóstico: os quatro achados críticos são sustentados exclusivamente por estudos de 2024-2025. O que se perdeu foram os números cuja idade os tornava indefensáveis.

---

## 3. AS 7 PERDAS ESTRUTURAIS

| # | Perda | Magnitude | Fonte · data | Sev. |
|---|---|---|---|---|
| 1 | Paradas planejadas excedem o turno | 28.178 s vs. 26.400 s = **106,7 %** | E6 · 05/25 | 🔴 |
| 2 | 79 % do trabalho manual não agrega valor | 21,2 % AV · 46,7 % NNAV · 32,1 % D | E1 · 04/24 | 🔴 |
| 3 | Inspeções e registros = 59,2 % das perdas | 16.700 s/turno (só a inspeção da montagem: 7.000 s) | E6 · 05/25 | 🔴 |
| 4 | Gargalo sem capacidade nominal para o takt | 2.856 vs. 3.086 pç/dia = **−7,4 %** | E6 · 05/25 | 🔴 |
| 5 | Desbalanceamento extremo da célula | Op. Montagem **136,9 %** vs. 4 ops. a 22-29 % | E6 · 05/25 | 🟠 |
| 6 | Montagem: 85 % do tempo sem valor | 15,0 % AV · 61,3 % necessário · 23,7 % D | E7 · 06/25 | 🟠 |
| 7 | Lead time de 14 dias com 0,007 % de VA | 20.347 min · 98,19 % de espera | E2 · 05/24 | 🟡 revalidar |

### As três alavancas — nesta ordem, obrigatoriamente

| # | Alavanca | Ataca | Impacto calculado |
|---|---|---|---|
| **1** | **MeasurLink** no gargalo e depois na linha | #1 #3 #7 | Perdas **106,7 % → 75,1 %** · eficiência **69,2 % → ~85 %** · R$ 270.284 |
| **2** | **Liberar capacidade no pino** (SMED + eliminar deslocamento e marcação) | #4 | Fechar o déficit de **230 pç/dia** |
| **3** | **Rebalancear** célula e montagem | #2 #5 #6 | Célula 5 → 4 ops. reais · montagem 5 → 4 postos (**+18,6 %**) |

> **Por que a ordem é obrigatória:** as atividades de controle valem **18,65 s/pç = 62,2 % do takt de 30 s**. Sem eliminá-las, a célula precisa de 89,18 ÷ 30 = **3 operadores no mínimo absoluto**, e todo cenário enxuto da planilha é ficção.

---

## 4. A EVIDÊNCIA, ESTUDO A ESTUDO

### 4.1 E1 · GBO TERMINAL — **17 e 18/04/2024**
*Alexandre Kichler Martins · 34 eventos cronometrados · dados de setup e eficiência coletados em março e abril de 2024*

| Parâmetro | Valor |
|---|---|
| Demanda · dias úteis | 62.332 pç/mês · 27 dias · 769,53 pç/turno |
| **Takt** | **37,425 s** (28.800 ÷ 769,53) |
| **Trabalho manual total** | **59,763 s/pç** (soma dos 34 eventos) |
| **Operadores** | 59,763 ÷ 37,425 = **1,60 → 2** |
| **Eficiência de campo** | **69,2 %** |
| Capacidade teórica | 109,09 pç/h · 70.691 pç/mês → folga de 13,4 % sobre a demanda |

**Para onde vai o tempo:** AV **12,667 s (21,2 %)** · NNAV **27,909 s (46,7 %)** · Desperdício **19,187 s (32,1 %)**. **Apenas 4 das 34 atividades agregam valor** — todas são abastecimento de máquina.

**Pareto — 8 atividades = 63,4 % do tempo:**

| Atividade | s/pç | % | Classe | Alavanca |
|---|---|---|---|---|
| **Deslocamento** | 10,000 | 16,7 % | D | Layout / arranjo celular |
| Abastecimento Equiptop | 6,667 | 11,2 % | AV | Otimizar |
| **Inspeção pino projetor** | 5,000 | 8,4 % | NNAV | **MeasurLink** |
| Marcar peça com marcador | 4,000 | 6,7 % | D | Laser / poka-yoke |
| Setup Caixa | 4,000 | 6,7 % | NNAV | SMED |
| Setup Equiptop | 3,720 | 6,2 % | NNAV | SMED |
| Desabastecimento Equiptop | 2,500 | 4,2 % | NNAV | Automação de descarga |
| Abastecimento Pino | 2,000 | 3,3 % | AV | Otimizar |
| **Subtotal** | **37,887** | **63,4 %** | | |

> Eliminando só as duas de classe **D** desse topo (deslocamento 10 s + marcação 4 s), o trabalho manual cai para **45,76 s** e os operadores de 1,60 para **1,22**. Eliminando todo o desperdício **+ metade do NNAV**: 26,62 s → **1 operador com 29 % de folga**.

### 4.2 E2 · SHINGO AV/NAV — **atualizado em 22/05/2024** ⚠

Lead time **20.347 min = 14,13 dias** para **1,43 min de processamento** → **VA de 0,00703 %**, com **98,19 % do tempo em espera por processamento** (19.980 min) e 1,77 % em espera de lote.

> É um problema de **lote e sincronização, não de velocidade de máquina**: reduzir o processamento de 1,43 min para 0,7 min mudaria o lead time em 0,0035 %. Número **a revalidar** antes de qualquer uso decisório (arquivo criado em 2022).

### 4.3 E3 · Tempos Pressmatik — **01 a 04/07/2024**
*Laiza Borges da Silva · cronometragem direta de 4 arranjos*

| | Cenário 1 | Cenário 3 | Cenário 4 | **Cenário 5** |
|---|---|---|---|---|
| Ciclo (s) | 46,88 | 42,15 | 36,16 | **34,26** |
| Entrega (pç/h) | 76,79 | 85,41 | 99,56 | **105,08** |
| Ganho acumulado | — | +11,2 % | +29,6 % | **+36,8 %** |

**Takt alvo 31,50 s → gap remanescente de 2,76 s (8,8 % acima).**

O elemento **"Caixinha"** é o maior do cenário vencedor (**12,22 s**) e o mais instável do estudo: **7,72 → 15,80 → 12,94 → 12,22 s** entre cenários (amplitude de 105 %). A porca também oscila 185 % e a etiqueta 111 %. A caixa master rateia 0,830 s (montagem) + 1,234 s (finalização) por peça, sobre lote de 18.

> **O gap de 2,76 s cabe inteiro dentro da variabilidade do encartuchamento. Padronizar esse único elemento fecha o takt sem investimento.**

### 4.4 E4 · Projeto de Capabilidade / MeasurLink — **06 a 13/08/2024**
*Paulo Frosi · Dieferson Duarte Antunes · base de cálculo: 12 meses reais (06/2023 a 06/2024)*

**O que muda:** registro em papel (**FO021**) + instrumentos analógicos + arquivo físico → coleta digital automática, alerta e bloqueio de máquina por peça fora de tolerância, arquivamento digital. Meta declarada: **−30 % de sucata operacional**, base para os projetos "F4" e "Rumo ao Defeito Zero".

| Investimento (R$ 56.419,16) | Ganhos (R$ 270.283,72) |
|---|---|
| Licenças (2) 30.000 · instrumentos 14.979,16 · PC 5.000 · ponto de rede 2.000 · CAL 1.800 · energia 1.200 · nobreak 600 · mesa 500 · leitor 300 · HDMI 40 | **Pontuais R$ 107.770** (capabilidade 24 h → 4 h = 105.600 · sucata 2.170) · **Riscos evitados R$ 161.832** (desvios e retrabalho 61.644 + 88.660 · sucata 11.528) · **Constantes R$ 681,72/mês** |

**Retorno:** só o ganho pontual já supera o investimento → **ROI de +91 % no primeiro ciclo**; com riscos evitados, **4,8× o investimento**.
**Fases:** 1ª **máquina gargalo em 15 dias**, 2ª linha TD10 completa em **90 dias**, 3ª demais células (Projeto F4, **R$ 847.000** no total da fábrica — o TD10 é o maior unitário porque carrega licenças e servidor, **é o investimento habilitador**).
**Piloto de 45 dias sem custo**, cedido pela Mitutoyo; suporte remoto gratuito (Mitutoyo e 3D Metrologia).

| ⚠ Dois alertas sobre este estudo |
|---|
| Os requisitos citam **SQL Server 2014/2016/2017 e Windows 8/10** — em fim de suporte em 2026. **Revalidar a especificação antes do CAPEX.** |
| O ganho de capabilidade (R$ 112.640/máquina) usa **128 pç/h** no gargalo; o E6 (mai/25) registra **119 pç/h** → o valor correto é **R$ 104.720** (−7,0 %). O caso de negócio segue válido. |

**Riscos declarados sem mitigação orçada:** interligação software ↔ CNC para bloqueio de máquina e integração de instrumentos de outros fabricantes.

### 4.5 E5 · GBO TD10 Rev06-1 (Estudo de Viradas) — **04/05/2025**

Traz dois cenários que **não existem na Rev07** — `NOVO LAYOUT` e `NOVO LAYOUT (2)`, ambos com 4 operadores, takt 28 s e **carga de 69,03 s** (ocupação máxima de 82,1 % e 85,8 %).

**O que mudou em 4 dias até a Rev07:** o **abastecimento da laminação (6 s) saiu do escopo** da célula e criou-se a distinção entre operar **com e sem WIP de caixa** (Métodos 1 e 2), derrubando a carga de 69,03 s para 57,53–63,03 s. A Rev07 é a versão vigente.

### 4.6 E6 · GBO TD10 Rev07 — **08/05/2025** ⭐ MODELO VIGENTE
*18 abas · capacidades, simulação horária de WIP, 10 cenários, perdas. Há **duas cópias byte-idênticas** no repositório (MD5 `0303913a41a23d4007bc15ff4d509952`).*

**Capacidade por operação (aba `Planilha4`):**

| Operação | pç/h | Horas | **pç/dia** |
|---|---|---|---|
| **PINO** | **119** | 24 | **2.856** ← gargalo |
| EQUIPTOP | 146 | 21 | 3.066 |
| CAIXA (2 máq.) | 206 | 21 | 4.326 |
| MONTAGEM | 150 | 21 | 3.150 |
| EMBALAGEM | 150 | 21 | 3.150 |

**O gargalo não suporta o takt adotado pela própria planilha:**

| Takt | Demanda implícita | Capacidade do pino | Situação |
|---|---|---|---|
| **28 s** | 3.085,7 pç/dia | 2.856 | **−229,7 pç/dia (−7,4 %)** ❌ |
| **30 s** | 2.880,0 pç/dia | 2.856 | −24 pç/dia (−0,8 %) ⚠ margem zero |

> Aplicando a eficiência real de 69,2 %, a capacidade cai para **1.976 pç/dia — déficit de 36 %**. Todo cenário de balanceamento desta planilha pressupõe uma capacidade que a própria planilha mostra não existir.

**Perdas de disponibilidade — o achado central:**

| Bloco | Tempo/turno | % das perdas | Quem ataca |
|---|---|---|---|
| **Inspeções** (5 tipos; só a da montagem = 7.000 s) | **13.340 s** | **47,3 %** | **MeasurLink** |
| **Viradas** (2 × 3.600 s) | 7.200 s | 25,6 % | Nivelamento |
| **Setups** (pino 720 · Equiptop 1.758 · caixa 1.800) | 4.278 s | 15,2 % | SMED |
| **Registros** (diário de bordo 2.880 + quadro 480) | 3.360 s | 11,9 % | **MeasurLink** |
| **TOTAL** | **28.178 s** | 100 % | |
| *Tempo disponível por turno* | *26.400 s* | → **razão 106,7 %** | |

> O MeasurLink endereça **16.700 s = 59,2 % das perdas**. Eliminando metade desse bloco, a razão cai de **106,7 % para 75,1 %**.

**Os 10 cenários, recalculados célula a célula** (soma das colunas de operador ÷ takt declarado na aba — matriz completa no Anexo A):

| Cenário | Ops. | Takt | Carga (s) | Ocup. máx. | Controle? |
|---|---|---|---|---|---|
| **ESTADO ATUAL** | 5 | 30 | 71,42 | **136,9 %** ❌ | Não |
| BALANCEADO | 5 | 30 | 89,18 | 85,5 % | **Sim** |
| **BALANCEADO (2)** ⭐ | 5 | 30 | 89,18 | **74,1 %** ✅ | **Sim** |
| MÉTODO 1 | 4 | 28 | 57,53 | 69,6 % | Não |
| MÉTODO 2 (com WIP CX) | 4 | 28 | 63,03 | 85,8 % | Não |
| NOVO LAYOUT 3 OP / CEN 2 | 3 | 28 | 71,53 | 94,6 % / 96,4 % ❌ | Não |
| CENÁRIO 1 / 2 / 3 | 3 | 28 | 72,53 | **99,5 %** / 95,2 % / 95,2 % ❌ | Não |

**No ESTADO ATUAL o Operador de Montagem carrega 41,08 s — 57,5 % da célula sozinho, 136,9 % do takt — enquanto os outros quatro somam 30,34 s e ficam abaixo de 29 %.** São ~89 s de ociosidade por ciclo distribuídos em 4 pessoas.

**As atividades de controle, que só o BALANCEADO (2) inclui:**

| Inspeção pino | Insp. Equiptop | Insp. caixa 1/25 | Insp. caixa 1/50 | **Insp. montagem** | Diário (6×) | Quadro | **TOTAL** |
|---|---|---|---|---|---|---|---|
| 1,083 | 1,360 | 0,367 | 2,040 | **6,800** | 6,000 | 1,000 | **18,650 s/pç** |

> **18,65 s/pç = 62,2 % do takt de 30 s.** É a prova numérica de que o MeasurLink é pré-requisito para qualquer redução de quadro. Somando o controle aos cenários de 3 operadores, a carga vai a ~90 s → **4 operadores**, não 3.

**Por que nenhum cenário de 3 operadores se sustenta:** (1) ignoram os 18,65 s de controle; (2) ocupação de 94–99,5 % é insustentável com variabilidade — a prática recomenda teto de 85 %; (3) o takt de 28 s pressupõe 3.086 pç/dia que o gargalo não entrega.

**Simulação horária de WIP** (ciclo que se repete a cada 8 h): a embalagem fica **6 horas com produção zero** acumulando até **249 peças** à frente; o Equiptop para **2 horas** com 119 peças represadas; a montagem para **4 horas** com até 258 peças. Do pino à embalagem, **3.509 peças ficam retidas (−9,1 %)**. O WIP **oscila ciclicamente em vez de estabilizar**, alternando falta de peça e bloqueio nas mesmas estações — assinatura de sistema **não nivelado**.

**Comparativo de produtividade** (aba `Planilha1`): média de 1.248,5 contra 1.970,25 peças = **razão de 63,4 %**, próxima dos 69,2 % de eficiência de E1 — os dois estudos se corroboram, e indicam **+57,8 % de produção possível com a mesma estrutura**.

### 4.7 E7 · Ferramenta GBO + Yamazumi — **13/06/2025** ⭐ O MAIS RECENTE
*David Avila Teixeira (Engenharia) · produto 335272 · 46 atividades por análise de vídeo · declarado 03/03/2025, salvo 13/06/2025*

> ⚠ **Escopo diferente:** trata da **montagem da família MTD inteira** (230.000 pç/mês, takt **8,217 s**), não do TD10 isolado. Complementar — mas os números **não podem ser misturados** com os de E1/E6.

| Posto (atual) | Movim. | Tméd ajust. (s) | Ocupação | Desperdício |
|---|---|---|---|---|
| OP1 Fechamento + Gravação | 6 | 6,473 | 78,8 % | 20,9 % |
| OP2 Guarda-pó | 7 | 6,489 | 79,0 % | 0 % |
| OP3 Saco plástico | 4 | 3,772 | 45,9 % | 33,4 % |
| **OP4 Cartucho** | 7 | **7,837** | **95,4 %** | **41,4 %** ❌ |
| OP5 **Master** | **22** | 6,428 | 78,2 % | 23,2 % |

Do total de 28,991 s: **AV 4,362 s (15,0 %) · necessário 17,761 s (61,3 %) · desperdício 6,868 s (23,7 %)**.

**A proposta de 4 postos** elimina ~2,94 s (todo o grampeamento manual, o check com pincel atômico, arrumação de cartuchos e espera) e declara: lead time 28,99 → **24,265 s**, capacidade 556,13 → **659,46 pç/h (+18,6 %)**, eficiência 88,20 → **94,64 %**, desperdício 23,7 → **15,0 %**, **5 → 4 postos**.

| ❌ O erro técnico | ✅ A correção |
|---|---|
| Consolidar **Cartucho + Master** no OP4 dá **10,163 s = 123,7 % do takt** — pior que o gargalo original (7,837 s). A capacidade real seria **3.600 ÷ 10,163 = 354 pç/h**, e não 659 — **46 % abaixo do anunciado**. | Transferir ~**2,53 s** de etiquetagem e abastecimento do OP4 para o **OP3**, que tem 4,46 s de folga: **OP3 ≈ 6,26 s (76,2 %) · OP4 ≈ 7,66 s (93,2 %)** — ambos abaixo do takt. O OP4 a 93,2 % ainda é alto: a solução robusta é **automatizar o fechamento da caixa master**. |

**Dois alvos óbvios revelados pelo estudo:**
- **Posto MASTER:** 22 das 46 atividades (47,8 %) em 5,59 s, **coeficiente de fadiga 13,04 % — 2,7× os demais postos — e zero atividades que agregam valor.** Maior risco ergonômico e maior alvo de automação da linha.
- **Etiquetagem:** 5 atividades distintas somando **1,954 s/pç = 23,8 % do takt**. Um aplicador automático é provavelmente o melhor retorno isolado da montagem.

### 4.8 E8 e E9 · Trabalhos padrão vigentes — **fev e abr/2024**

**TPO040 — Pino / Torno CNC (27/02/2024):** ciclo = tempo de máquina + 7 s (TD10/20/30); 14 s de tempo homem em 10 passos; usinagem de 15 s. Mantém um **sistema de gestão visual por cor padronizado: VERDE = setup · AMARELO = inspeção · VERMELHO = sucata**. Inspeção remetida ao **PC001**.

**TPO043 — Embalagem guarda-pó (Rev. 1, 01/04/2024):** 11 operações, da impressão de etiquetas (IT 147) à selagem e ao fechamento da caixa master.

> ⚠ **Conflito direto com E7:** a **operação 11 deste padrão vigente** ("check com pincel atômico") é exatamente a atividade classificada como **desperdício e marcada para eliminação** no estudo mais recente. **Eliminá-la exige revisar e reaprovar o TPO043 (Rev. 2).**

**Documentos citados, mas ausentes do repositório:** **PC001** (plano de controle do gargalo) 🔴 · **FO021** (formulário de inspeção, alvo do MeasurLink) 🟠 · **IT 215** e **IT 147** 🟡.

---

## 5. DIVERGÊNCIAS A RESOLVER ANTES DE INVESTIR

| # | Item | Valores em conflito | Impacto | Prior. |
|---|---|---|---|---|
| 1 | **Inserir bucha** | **2,00 s** (cenários futuros E6) ↔ **8,22 s** (ESTADO ATUAL de E6 **e** Cenário 1 de E3) — **+311 %** | 6,22 s/pç = **22,2 % do takt**. A coincidência entre E3 e o estado atual sugere que **8,22 s é o medido e 2,00 s é meta não validada** — o que tornaria **todos** os cenários futuros otimistas | 🔴 |
| 2 | **Setup do pino** | 594 s (E1) ↔ 720 s (E6 `PERDAS`) ↔ 1.800 s (E6 `Planilha2`) — **+203 %** | Afeta direto a capacidade do gargalo | 🔴 |
| 3 | **Tempo de virada** | 7.200 s ↔ 10.800 s — **dentro do mesmo arquivo E6** | Razão de perdas sobe de **106,7 % para 120,3 %** | 🔴 |
| 4 | **Capacidade do gargalo** | 119 pç/h (E6) ↔ 128 pç/h (E4) — +7,6 % | Ganho de capabilidade cai de R$ 112.640 para **R$ 104.720** | 🔴 |
| 5 | **Takt time** | 37,43 / 31,50 / 30 / 28 / 8,22 s | Não são erros — são escopos e épocas diferentes. Mas **nenhum documento declara escopo e data-base**, o que facilita o uso cruzado indevido | 🟠 |

**Evolução do takt (contexto do item 5):**

| 04/2024 (E1) | 07/2024 (E3) | 05/2025 (E6) | 05/2025 (E5/E6) | 06/2025 (E7) |
|---|---|---|---|---|
| **37,43 s** TD10 | 31,50 s Pressmatik | 30,00 s célula | **28,00 s** cenários futuros | 8,22 s montagem MTD |

> **−25,2 % em 13 meses = +33,7 % de demanda. A capacidade do gargalo não acompanhou:** em abr/2024 havia folga teórica de 13,4 %; em mai/2025 há déficit nominal de 7,4 %.

---

## 6. PLANO DE AÇÃO

### FASE 0 — Travar os parâmetros · 0–30 dias · custo ≈ 0
Definir valor único para **bucha, setup do pino, virada e capacidade do gargalo** (§5); declarar escopo e data-base de cada takt; confirmar se o `GBO Montagem.xlsx` foi atualizado em set/2026. **Entregável: "GBO TD10 Rev08" — versão única, com data, autor e escopo no cabeçalho.**

### FASE 1 — MeasurLink · 30–135 dias · R$ 56.419,16
Rodar o **piloto gratuito de 45 dias**; **revalidar a especificação técnica** (SQL Server / Windows em fim de suporte); corrigir o caso de negócio para 119 pç/h; liberar CAPEX; **gargalo em 15 dias, linha completa em 90**; digitalizar diário de bordo e quadro (3.360 s/turno); ativar alerta e bloqueio por fora de tolerância.
**Meta: perdas 28.178 → ~17.500 s · razão 106,7 % → 66,3 % · eficiência 69,2 % → ~85 %.**

### FASE 2 — Liberar o gargalo · 60–150 dias · custo baixo
**SMED nos 3 setups** (4.278 s/turno → ~2.139 s); eliminar a **marcação com marcador industrial** (4,00 s/pç) por laser ou poka-yoke; atacar os **10,00 s/pç de deslocamento** por arranjo de posto; nivelar o sequenciamento para reduzir as **viradas** (7.200 s/turno).
**Meta: fechar o déficit de 230 pç/dia no takt de 28 s.**

### FASE 3 — Rebalancear a célula · 135–180 dias · custo ≈ 0
Recalcular o GBO **sem as atividades de controle eliminadas pelo MeasurLink**, partindo do **BALANCEADO (2)** (único com controle incluído, ocupação máxima de 74,1 %). Com ~12 s/pç de controle eliminados, a carga cai de 89,18 s para ~77 s → **3 operadores viáveis com folga**. **Não adotar os CENÁRIOS 1-3 como estão.** Corrigir imediatamente o ESTADO ATUAL (Op. Montagem a 136,9 % com quatro colegas abaixo de 29 %).

### FASE 4 — Rebalancear a montagem · 150–200 dias · custo ≈ 0 a baixo
Aplicar a **correção do OP4** (§4.7) e validar OP3 ≈ 6,26 s / OP4 ≈ 7,66 s; avaliar **aplicador automático de etiquetas** (1,954 s/pç = 23,8 % do takt) e **automação da caixa master** (elimina o risco ergonômico do OP5); **revisar o TPO043 (Rev. 2)**.
**Meta: 5 → 4 postos · 556 → 659 pç/h · desperdício 23,7 % → 15,0 %.**

### FASE 5 — Pressmatik e sustentação · contínuo · custo ≈ 0
**Padronizar o elemento "Caixinha"** (12,22 s, variação de 105 %) para fechar o gap de 2,76 s; ampliar as cronoanálises de 6 para ≥ 10 ciclos; **refazer o MFV (Rev. 01)**; atualizar a referência antropométrica e aplicar a NR-17 vigente; avaliação ergonômica formal do posto MASTER; replicar para **TD20/TD30/TD40** (R$ 124.257,48 restantes na família).

### Resumo financeiro

| Fase | Investimento | Retorno | Prazo |
|---|---|---|---|
| 0 Parâmetros | ≈ 0 | Habilitador | 30 d |
| **1 MeasurLink** | **R$ 56.419,16** | R$ 107.770 pontual + R$ 161.832 em risco evitado + R$ 681,72/mês | 135 d |
| 2 Gargalo | baixo (interno) | ~2.139 s/turno + até 14 s/pç de desperdício | 150 d |
| 3 Célula | ≈ 0 | 5 → 3 operadores/turno | 180 d |
| 4 Montagem | ≈ 0 a baixo | −1 posto · +18,6 % de capacidade | 200 d |
| 5 Sustentação | ≈ 0 | Fechamento do takt | contínuo |
| **TOTAL** | **R$ 56.419,16** | **> R$ 270.000 + redução de quadro** | **~7 meses** |

> Não foi incluído o investimento de R$ 20.810,27 do projeto de fluxo por família: as ordens de compra são de **2022**, fora do corte, e não há evidência recente sobre seu status.

---

## 7. O QUE PRECISA SER REVALIDADO

| # | Item | Por quê | Prior. |
|---|---|---|---|
| 1 | **Demanda e takt atuais** | O dado mais recente é de mai/2025; a tendência histórica é de +25 %/ano | 🔴 |
| 2 | **Eficiência atual** | Os 69,2 % são de mar-abr/2024 — 2,5 anos atrás | 🔴 |
| 3 | **Lead time (E2)** | Pode ter sido herdado da versão de 2022 | 🔴 |
| 4 | **Status do CAPEX do MeasurLink** | O projeto é de ago/2024; não há notícia de liberação ou do piloto | 🔴 |
| 5 | **Especificação técnica do MeasurLink** | SQL Server 2014-2017 e Windows 8/10 em fim de suporte | 🔴 |
| 6 | **PC001 e MFV atualizado** | Faltam o plano de controle **do gargalo** e um MFV posterior a 2011 | 🔴 |
| 7 | **IROG real do gargalo** | Nenhum estudo recente mede disponibilidade × performance × qualidade | 🟠 |
| 8 | **`GBO Montagem.xlsx` e layout físico vigente** | Confirmar a edição de set/2026; nenhum documento recente registra o arranjo atual | 🟠 |

**Limitações metodológicas a corrigir nos próximos estudos:** amostras de 6 ciclos em E3 (o cenário vencedor tem a menor amostra) · coluna "Ritmo" = 1,00 em todas as 46 atividades de E7, o que impede chamá-los de tempo padrão formal · coeficiente de fadiga sem referência de tabela · rateio de setup sobre lote fixo de 450 peças em E1 · cenários sem atividades de controle em E5/E6 · ausência de cabeçalho com data e autor nas planilhas (as datas só foram recuperáveis via metadados).

**Higiene do repositório:** excluir `!!Cópia de Cópia de GBO - TD10 - Rev07.xlsx` (duplicata exata), `~$Tempos Pressmatik.xlsx` (lock do Excel) e `Thumbs.db`; adotar a convenção `GBO_TD10_RevXX_AAAA-MM-DD_autor.xlsx`; renomear abas `Planilha1/2/3/4`.

---

## ANEXO A — Matriz de atividades por cenário (E6 · Rev07 · 08/05/2025)

| Atividade | Estado Atual | Balanc. | Balanc. 2 | Mét. 1 | Mét. 2 | 3OP Cen2 | Cen 3OP | Cen 1 | Cen 2 | Cen 3 |
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
| **Subtotal operação** | **71,42** | 70,53 | 70,53 | **57,53** | **63,03** | **71,53** | **71,53** | **72,53** | **72,53** | **72,53** |
| Atividades de controle | — | **18,65** | **18,65** | — | — | — | — | — | — | — |
| **CARGA TOTAL** | **71,42** | **89,18** | **89,18** | 57,53 | 63,03 | 71,53 | 71,53 | 72,53 | 72,53 | 72,53 |
| Operadores · takt | 5 · 30 | 5 · 30 | 5 · 30 | 4 · 28 | 4 · 28 | 3 · 28 | 3 · 28 | 3 · 28 | 3 · 28 | 3 · 28 |
| **Ocupação máxima** | **136,9 %** | 85,5 % | **74,1 %** | 69,6 % | 85,8 % | 96,4 % | 94,6 % | **99,5 %** | 95,2 % | 95,2 % |

## ANEXO B — Rastreabilidade

| Cód. | Arquivo | Data do estudo | Identificação |
|---|---|---|---|
| E1 | `GBO TERMINAL.xlsx` | 17-18/04/2024 | aba `TD10` |
| E2 | `SHINGO - AV NAV.xlsx` | 22/05/2024 (criado 07/04/2022) | aba `SHINGO - F3` |
| E3 | `Pressmatik/Tempos Pressmatik.xlsx` | 01-04/07/2024 | abas `CENÁRIO 1/3/4/5`, `COMPARAÇÃO`, `MASTER` |
| E4 | `01 - PROJETO DE CAPABILIDADE TD10( Measure Link ) - atualizado 06.08.24.pptx` | 06-13/08/2024 | 10 slides |
| E5 | `GBO - TD10 - Rev06-1 - ESTUDO DE VIRADAS - DIA A DIA.xlsx` | 04/05/2025 | abas `NOVO LAYOUT`, `NOVO LAYOUT (2)` |
| E6 | `Cópia de Cópia de GBO - TD10 - Rev07.xlsx` | 08/05/2025 | MD5 `0303913a41a23d4007bc15ff4d509952` · 18 abas |
| E7 | `Ferramenta GBO + YAMAZUMI - Rev1 ( Manipulação 4 operadores).xlsm` | 03/03/2025 → 13/06/2025 | 7 abas |
| E8 | `trabalhopadrao/TPO040.pdf` | 27/02/2024 | 1 página |
| E9 | `trabalhopadrao/TPO043.pdf` | Rev. 1 — 01/04/2024 | 2 páginas |

*Datação por metadados internos (`docProps/core.xml`, `/CreationDate` do PDF, `SummaryInformation` do OLE), cruzada com as datas declaradas no conteúdo. Cenários de balanceamento recalculados célula a célula a partir das abas originais.*

---

**FIM** · *Base exclusiva: 9 estudos realizados entre 27/02/2024 e 13/06/2025. As divergências da §5 devem ser resolvidas antes de executar o plano da §6.*
