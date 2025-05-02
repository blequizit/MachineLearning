# 🚗 Análise Exploratória II - Preço de Carros

Este repositório contém um projeto de Análise Exploratória de Dados (EDA) aplicado a um conjunto de dados de preços de carros, com o objetivo de entender os fatores que influenciam no valor dos veículos.

---

## 🎯 Objetivo

O objetivo deste projeto é:

- Aplicar técnicas de Análise Exploratória de Dados (EDA) para compreender as características dos veículos e suas relações com o preço final.
- Identificar padrões e correlações entre variáveis, como tamanho do motor, peso e tipo de tração, que influenciam o preço dos carros.
- Visualizar as distribuições e relações das variáveis através de gráficos e diagramas.
- Analisar a influência de variáveis categóricas, como tipo de combustível e tipo de carroceria, no preço.

---

## 📁 Estrutura do Repositório

- `Analise Descritiva.ipynb`: Notebook com toda a análise exploratória dos dados.
- `CarPrice_Assignment.csv`: Dataset utilizado na análise.
- `README.md`: Este arquivo com explicações sobre o projeto.

---

## 📊 Etapas Realizadas

### 📌 Leitura e Limpeza de Dados
- Leitura do dataset com `pandas`.
- Estatísticas descritivas com `df.describe()`.
- Verificação de dados ausentes e duplicados.

### 📌 Análise Univariada
- Análise da distribuição da variável `price`.
- Visualização de distribuições de variáveis categóricas e numéricas com histogramas e gráficos de barras.

### 📌 Análise de Correlação
- Geração de uma matriz de correlação para identificar variáveis relacionadas.
- Visualização das correlações com o gráfico `px.imshow`.

### 📌 Análise Bivariada
- Exploração da relação entre `enginesize` e `price`.
- Boxplots entre `price` e variáveis categóricas como `carbody`, `fueltype`, `aspiration`, `drivewheel`, `cylindernumber`.
- Análise das médias de preço por categoria com gráficos de barra.

### 📌 Análise de Consumo (citympg)
- Relação entre variáveis como `enginesize`, `horsepower`, `curbweight` e `citympg`.
- Boxplots e scatterplots para comparar o consumo por tipo de tração e número de cilindros.

---

## 🛠️ Bibliotecas Utilizadas

- `pandas`
- `numpy`
- `plotly.express`
- `plotly.graph_objects`
- `seaborn`
- `matplotlib`

---

## 📂 Requisitos

```bash
pip install pandas numpy plotly seaborn matplotlib
```

---

## Contato

Autor: Eduardo Ferreira  
Email: eduds1010@gmail.com

---

## Agradecimento

Agradecimento ao professor Leandro Romualdo da Silva ministrou aulas sobre o conteúdo.
