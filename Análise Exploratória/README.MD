# 📊 Análise Exploratória I - Conhecendo os Dados

Este repositório apresenta uma análise exploratória de dados (EDA) com foco em compreender a estrutura, distribuição e relações de variáveis de um dataset utilizado em projetos de Machine Learning.

---

## 🎯 Objetivo

Realizar uma análise inicial dos dados contidos no arquivo `dataset_armageddon_final_corrected.csv`, com o intuito de:

- Identificar a estrutura geral do dataset
- Visualizar distribuições de variáveis numéricas e categóricas
- Detectar outliers
- Analisar correlações entre variáveis numéricas
- Observar relações entre variáveis através de gráficos bivariados
- Gerar um relatório automático com o `pandas_profiling`
- Criar uma estrutura base de controle financeiro com `pandas` e `xlsxwriter`

---

## 📁 Estrutura do Repositório

- `Analise Exploratória I.ipynb`: Notebook contendo todo o processo de análise exploratória.
- `dataset_armageddon_final_corrected.csv`: Dataset analisado.
- `Armageddon Analysis.html`: Relatório gerado com o `pandas_profiling`.
- `controle_financeiro_template.xlsx`: Modelo de controle financeiro automatizado em Excel.
- `README.md`: Este arquivo com explicações do projeto.

---

## 📊 Etapas Realizadas

### 📌 Leitura e Informações Iniciais
- Leitura do dataset com `pandas`
- Exibição de amostra com `df.sample()`
- Resumo estatístico com `df.describe()`
- Verificação de valores ausentes

### 📌 Visualização Univariada
- Histogramas para variáveis numéricas
- Gráficos de barras para variáveis categóricas

### 📌 Detecção de Outliers
- Boxplots para variáveis numéricas

### 📌 Análise de Correlação
- Geração de matriz de correlação
- Visualização com `seaborn.heatmap`

### 📌 Análise Bivariada
- `scatterplots` entre variáveis numéricas
- `boxplots` entre variáveis numéricas e categóricas

### 📌 Geração de Relatório com Pandas Profiling
- Criação de relatório interativo com `ProfileReport`

### 📌 Estrutura de Arquivo Financeiro (Bônus)
Geração de três abas:
- `database`
- `Resumo Mensal` (com fórmulas automatizadas)
- `Projeção`

Criação do arquivo Excel `controle_financeiro_template.xlsx` com `xlsxwriter`

---

## 🛠️ Bibliotecas Utilizadas

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `pandas_profiling`
- `xlsxwriter`

---

## 📂 Requisitos

```bash
pip install pandas matplotlib seaborn pandas-profiling xlsxwriter
```

---

## 📄 Relatório Gerado

O relatório interativo da análise pode ser visualizado abrindo o arquivo Armageddon Analysis.html.

---

## Contato

Autor: Eduardo Ferreira  
Email: eduds1010@gmail.com

---

## Agradecimento

Agradecimento ao professor Leandro Romualdo da Silva ministrou aulas sobre o conteúdo.
