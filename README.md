# 📊 Análise de Dados — IEGM 2023 | Municípios do Ceará

Análise exploratória dos dados do **Índice de Efetividade da Gestão Municipal (IEGM)** referente ao ano de 2023, com foco nos municípios do Estado do Ceará, disponibilizados pelo **Tribunal de Contas do Estado do Ceará (TCE-CE)**.

---

## 📌 Contexto

O IEGM é uma ferramenta nacional idealizada pelo TCESP em 2015 e adotada por outros Tribunais de Contas do Brasil. Ele avalia a qualidade da gestão administrativa e a efetividade das políticas públicas municipais em sete áreas:

| Índice | Área |
|--------|------|
| I-Amb | Meio Ambiente |
| I-Cidade | Proteção das Cidades |
| I-Educ | Educação |
| I-Fiscal | Gestão Fiscal |
| I-Gov TI | Governança de TI |
| I-Saúde | Saúde |
| I-Plan | Planejamento |

A nota final de cada índice é classificada em faixas de **A (melhor)** a **E (pior)**.

---

## 🎯 Objetivos

1. Identificar qual município obteve a **melhor nota em cada uma das sete áreas** do IEGM
2. Analisar as **respostas enviadas** por esses municípios destaque para entender o que contribuiu para a boa nota
3. Identificar **qual nota cada resposta recebeu**, permitindo entender o que fez a diferença no desempenho de cada município

---

## 🗂️ Bases de Dados

| Arquivo | Descrição |
|--------|-----------|
| `geral_iegm_2023_TCECE_municipio.csv` | Notas finais de todos os municípios por área |
| `respostas_iegm_2023_TCECE_completo_nota.csv` | Respostas individuais de cada município com nota por questão |
| `calculo_iegm_2023_TCECE_completo.csv` | Cálculo detalhado das notas por área e município |

> Fonte: [TCE-CE — Tribunal de Contas do Estado do Ceará](https://www.tce.ce.gov.br)

---

## 🔍 Estrutura da Análise

### Análise 1 — Melhor Município por Área
Identificação do município com maior nota percentual em cada uma das sete áreas, com visualização gráfica comparativa.

### Análise 2 — Respostas dos Municípios Destaque
Extração e exibição das respostas enviadas por cada município campeão, mostrando quais questões foram respondidas e qual nota cada resposta recebeu.

### Curiosidade — Comparação: Sobral vs. Município Destaque
Ao longo da análise, foi possível observar que Sobral liderou em cinco das sete áreas do IEGM 2023. Nas áreas de Educação (Groaíras) e Planejamento (Caucaia), onde Sobral não ficou em primeiro lugar, foi feita uma comparação lado a lado das respostas dos dois municípios para identificar quais questões foram respondidas de forma diferente e como isso impactou a nota final.

---

## 🛠️ Tecnologias Utilizadas

- Python 3
- Pandas
- Matplotlib
- Seaborn
- Google Colab

---

## 📁 Outputs Gerados

- `melhores_por_area.png` — gráfico com os melhores municípios por área
- `respostas_i{area}_{municipio}.csv` — respostas de cada município campeão por área
