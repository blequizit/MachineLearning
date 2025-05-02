# 📊 Regressão Simples

Este repositório contém um projeto de regressão linear aplicada ao dataset `dataset_armageddon_final_corrected.csv`, com foco em entender a relação entre variáveis explicativas e a variável dependente através de modelos de regressão simples e múltipla.

---

## 🎯 Objetivo

O objetivo deste projeto é:

- Construir um modelo de regressão linear simples para prever o tempo de armageddon a partir da potência.
- Expandir o modelo para regressão linear múltipla com outras variáveis explicativas.
- Avaliar a performance do modelo utilizando métricas como R² e p-values.
- Realizar transformações em variáveis categóricas para otimizar a modelagem.
- Visualizar os resultados através de gráficos de dispersão e reta de regressão.

---

## 📁 Estrutura do Repositório

- `Regressão Simples.ipynb`: Notebook contendo todo o processo de construção e avaliação do modelo de regressão.
- `dataset_armageddon_final_corrected.csv`: Dataset utilizado para treinar os modelos de regressão.
- `README.md`: Este arquivo com explicações sobre o projeto.

---

## 📊 Etapas Realizadas

### 📌 Leitura e Preparação dos Dados
- Leitura do dataset com `pandas`.
- Visualização de amostras do dataset utilizando `df.sample()`.
- Transformação de variáveis categóricas com `LabelEncoder`.

### 📌 Construção do Modelo de Regressão Linear Simples
- Definição da variável dependente (`tempo_armageddon_s`) e da variável independente (`potencia`).
- Treinamento do modelo de regressão linear simples utilizando `statsmodels`.
- Análise do resumo estatístico e visualização do modelo com gráficos.

### 📌 Testes de Significância
- Aplicação do Teste F para avaliar a significância global do modelo.
- Análise dos p-values dos coeficientes para testar a significância das variáveis explicativas.

### 📌 Construção do Modelo de Regressão Linear Múltipla
- Expansão do modelo para incluir múltiplas variáveis explicativas como `peso` e `potencia`.
- Treinamento do modelo de regressão linear múltipla e análise de resultados.

### 📌 Visualizações
- Gráficos de dispersão e linha de regressão para observar as relações entre variáveis.

---

## 🛠️ Bibliotecas Utilizadas

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `sklearn`

---

## 📂 Requisitos

```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
```

---

## Contato

Autor: Eduardo Ferreira  
Email: eduds1010@gmail.com

---

## Agradecimento

Agradecimento ao professor Leandro Romualdo da Silva ministrou aulas sobre o conteúdo.
