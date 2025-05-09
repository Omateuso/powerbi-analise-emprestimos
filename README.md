# 📊 Análise de Empréstimos com Power BI

Este projeto consiste em um dashboard interativo desenvolvido no **Power BI**, com foco na análise de dados de **empréstimos financeiros**, aplicação de conceitos de estatística descritiva, classificação de risco e simulação de cenários com base em variações de taxas de juros.

## 🚀 Objetivo
Analisar o comportamento dos empréstimos aprovados, calculando métricas relevantes como juros acumulados, prazo médio e valores médios por finalidade. Além disso, simular os impactos da variação da taxa de juros sobre os empréstimos.

---

## 📁 Arquivos

- `loan_data.csv`: Base de dados principal dos empréstimos.
- `dashboard_emprestimos.pbix`: Arquivo do Power BI com as visualizações e medidas criadas.
- `README.md`: Descrição do projeto.

---

## 📌 Funcionalidades

### Página 1 – Visão Geral
- **Cartões** com:
  - Média do valor dos empréstimos
  - Média dos juros totais
  - Prazo médio em anos
  - Soma de juros totais
  - Total de empréstimos no ano anterior
- **Gráfico de barras empilhadas**: Distribuição dos empréstimos por classificação de risco
- **Gráfico de colunas clusterizado**: Valor médio de empréstimo por finalidade (Propouse)
- **Slicers**: Filtros por risco e finalidade

### Página 2 – Simulações e Tendências
- **Parâmetro personalizável**: Taxa de juros simulada
- **Gráfico de linhas**: Variação dos juros totais com base na taxa
- **Cartão**: Valor dos juros simulados
- **Gráfico de rosquinha**: Distribuição de empréstimos por finalidade
- **Gráfico de dispersão**: Relação entre valor do empréstimo e juros simulados
- **Tabela resumo**: Com propósitos, médias de valores, prazos, juros e risco

---

## 🧠 Métricas e Cálculos Importantes

- **Juros Totais**: `Loan_Amount × 0.05 × Loan_Term`
- **Classificação de Risco**:
  - Baixo: Parcelas abaixo de 15.000
  - Médio: Entre 16.000 e 30.000
  - Alto: Acima de 30.000
- **Loan Amount**: Parcela × Duração (em dias)
- **Loan Term (em anos)**: Duração (em dias) ÷ 365

---

## 🔧 Ferramentas e Tecnologias

- Power BI Desktop
- Linguagem **DAX** para medidas e colunas calculadas
- Tratamento de dados diretamente no Power BI

---

## 📌 Observações

- Os dados foram tratados para corrigir tipos de dados, formatar colunas de moeda, porcentagem e datas.
- O projeto permite uma análise flexível e visualmente rica sobre o comportamento de empréstimos.
