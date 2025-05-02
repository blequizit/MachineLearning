#  Projetos de Machine Learning

Este repositório contém diversos projetos de Machine Learning e Análise de Dados desenvolvidos em Python. Cada pasta apresenta um estudo específico com dataset, notebook e README próprios.

---

## 📁 Estrutura do Repositório

### 1. `Análise Exploratória`
🔍 **Análise inicial de dados**  
Projeto voltado à exploração de um dataset com foco na compreensão da estrutura, distribuição e correlações das variáveis. Inclui geração de relatório automático com `pandas_profiling` e construção de um controle financeiro em Excel como bônus.

- 📊 Visualização de variáveis numéricas e categóricas  
- 📈 Detecção de outliers e correlações  
- 📋 Geração de relatório com `pandas_profiling`  
- 📂 Criação de planilha financeira automatizada com `xlsxwriter`  

📎 **Arquivos**:
- `Analise Exploratória I.ipynb`
- `dataset_armageddon_final_corrected.csv`
- `Armageddon Analysis.html`
- `controle_financeiro_template.xlsx`

---

### 2. `Análise Exploratória II`
🚗 **Análise dos fatores que influenciam o preço de carros**  
Aplicação de técnicas de EDA para entender como variáveis como tamanho do motor, tipo de tração e tipo de combustível impactam o valor dos veículos.

- 📉 Análise univariada, bivariada e de correlação  
- 📌 Exploração de variáveis categóricas como `fueltype`, `carbody`, `drivewheel`  
- 📊 Visualizações com `plotly`, `seaborn` e `matplotlib`

📎 **Arquivos**:
- `Analise Descritiva.ipynb`
- `CarPrice_Assignment.csv`

---

### 3. `Regressão Linear`
📊 **Modelagem preditiva com regressão linear simples e múltipla**  
Modelo construído para prever o tempo de um evento chamado "armageddon" a partir de variáveis como potência e peso.

- 📈 Regressão linear simples e múltipla com `statsmodels`  
- 🧪 Testes estatísticos de significância (p-values, F-test)  
- 🔍 Visualização de dispersão e linha de regressão  

📎 **Arquivos**:
- `Regressão Simples.ipynb`
- `dataset_armageddon_final_corrected.csv`

---

### 4. `Ensemble Regressor`
🚀 **Modelos de Regressão com Técnicas Ensemble**  
Comparação de diversos algoritmos de ensemble (bagging e boosting) para prever o tempo de armageddon com alta performance.

- 🌲 Random Forest, Extra Trees  
- 🌟 Gradient Boosting, AdaBoost, XGBoost, LightGBM  
- 📊 Avaliação com métricas como MAE, MSE, RMSE, MAPE, R²  
- 💾 Salvamento dos modelos com `pickle` para reuso

📎 **Arquivos**:
- `Ensemble Regressor.ipynb`
- `dataset_armageddon_final_corrected.csv`

---

## 🛠️ Tecnologias Utilizadas

- Python 3  
- Pandas, NumPy  
- Seaborn, Matplotlib, Plotly  
- Statsmodels, Scikit-learn  
- XGBoost, LightGBM  
- Pandas Profiling, XlsxWriter  
- Pickle  

---

## 👨‍💻 Autor

Eduardo Ferreira  
📧 eduds1010@gmail.com  

---

## 🎓 Agradecimento

Agradecimento especial ao professor **Leandro Romualdo da Silva** pelas aulas e orientações nos projetos.

