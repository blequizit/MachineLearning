# Regressão Simples

Este repositório contém um projeto de regressão linear aplicada ao dataset `dataset_armageddon_final_corrected.csv`. O objetivo do projeto é construir um modelo de regressão simples e múltipla para entender a relação entre variáveis explicativas e a variável dependente.

🎯 **Objetivo**

O projeto visa:

- Aplicar técnicas de regressão linear simples e múltipla.
- Avaliar a performance do modelo utilizando métricas como R² e p-values.
- Realizar transformações em variáveis categóricas para otimizar o modelo.

📁 **Estrutura do Repositório**

- `Regressão Simples.ipynb`: Notebook contendo todo o processo de análise e construção dos modelos de regressão.
- `dataset_armageddon_final_corrected.csv`: Dataset utilizado para construir o modelo.
- `README.md`: Este arquivo com explicações sobre o projeto.

📊 **Etapas Realizadas**

1. **Leitura dos Dados**
   - Carregamento do dataset utilizando o `pandas`.
   - Visualização de amostras e resumo das variáveis.

2. **Regressão Linear Simples**
   - Definição da variável dependente (`tempo_armageddon_s`) e independente (`potencia`).
   - Ajuste do modelo de regressão linear simples utilizando `statsmodels`.
   - Análise do resumo estatístico e gráficos.

3. **Teste de Significância**
   - Teste F para avaliar a significância global do modelo.
   - Teste de significância para os coeficientes das variáveis preditoras.

4. **Regressão Linear Múltipla**
   - Expansão do modelo para incluir múltiplas variáveis explicativas como `peso` e `potencia`.
   - Ajuste e avaliação do modelo de regressão múltipla.

5. **Transformação de Variáveis Categóricas**
   - Conversão de variáveis categóricas utilizando `LabelEncoder` para inclusão no modelo.

6. **Visualização**
   - Gráficos de dispersão e reta de regressão para a análise da relação entre variáveis.
   - Visualização do impacto das variáveis explicativas sobre o tempo do armageddon.

🛠️ **Bibliotecas Utilizadas**

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `sklearn`

📂 **Requisitos**

Para rodar o código, instale as bibliotecas necessárias com o seguinte comando:

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
