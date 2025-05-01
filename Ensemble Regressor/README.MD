# Regressão com Modelos Ensemble

Este repositório apresenta uma análise preditiva utilizando algoritmos de **ensemble regressors** para prever o tempo de um evento denominado "armageddon", com base em um conjunto de variáveis explicativas. A abordagem envolve o uso de modelos como **Random Forest**, **Gradient Boosting**, **Extra Trees**, **AdaBoost**, **XGBoost** e **LightGBM**.

---

## 🎯 Objetivo

Desenvolver e comparar modelos de regressão baseados em técnicas de ensemble para prever o tempo (`tempo_armageddon_s`) com o melhor desempenho possível. O projeto inclui:

- Pré-processamento de dados
- Treinamento e avaliação de modelos
- Salvamento dos modelos treinados com `pickle`

---

## 📁 Estrutura do Repositório

- `Ensemble Regressor.ipynb`: Notebook com todo o pipeline de Machine Learning.
- `dataset_armageddon_final_corrected.csv`: Base de dados com variáveis utilizadas no modelo.
- Modelos `.pkl`: Arquivos serializados contendo os modelos treinados:
  - `lgbm_model.pkl`
  - `rf_model.pkl`
  - `et_model.pkl`
  - `gbm_model.pkl`
  - `xgb_model.pkl`
  - `ada_model.pkl`
- `README.md`: Este arquivo com explicações sobre o projeto.

---

## 📊 Dataset

O arquivo `dataset_armageddon_final_corrected.csv` contém variáveis de entrada (preditoras) e a variável-alvo `tempo_armageddon_s`.

As colunas categóricas foram convertidas para o tipo `category` e codificadas numericamente para utilização em modelos de machine learning.
---

### 🧾 Dicionário de Dados

Abaixo estão as descrições das colunas presentes no arquivo `dataset_armageddon_final_corrected.csv`:

| Coluna                   | Descrição                                                                 |
|--------------------------|---------------------------------------------------------------------------|
| **peso**                 | Peso do carro em quilogramas                                              |
| **potencia**             | Potência do motor em cavalos                                              |
| **velocidade_max**       | Velocidade máxima estimada do carro em km/h                              |
| **tipo_cambio**          | Tipo de câmbio utilizado (ex: Manual, Sequencial)                         |
| **tipo_pneu**            | Tipo de pneu utilizado (ex: Hoosier, Radial, Slick etc.)                  |
| **tipo_motor**           | Tipo do motor (ex: V6, V8, Inline etc.)                                   |
| **sobrealimentacao**     | Tipo de sobrealimentação (ex: Aspirado, Turbo, Supercharger)              |
| **carroceria**           | Material da carroceria (ex: Fibra, Metal etc.)                            |
| **tracao**               | Tipo de tração do veículo (ex: Dianteira, Traseira, 4x4)                  |
| **pista**                | Tipo de pista onde o teste foi realizado (ex: Pista Tratada, Asfalto etc.)|
| **titulos_armageddon**   | Número de títulos anteriores conquistados no evento "armageddon"          |
| **vitorias_lista_estado**| Número de vitórias em competições estaduais                              |
| **tempo_armageddon_s**   | Tempo total da corrida armageddon, em segundos (variável alvo)            |

---

## 🤖 Modelos Utilizados

### Bagging
- `RandomForestRegressor`
- `ExtraTreesRegressor`

### Boosting
- `GradientBoostingRegressor`
- `AdaBoostRegressor`
- `XGBRegressor` (XGBoost)
- `LGBMRegressor` (LightGBM)

Todos os modelos foram treinados com os parâmetros:
- `n_estimators=100`
- `random_state=42`

---

## 📐 Métricas de Avaliação

A função `assertividade()` retorna as seguintes métricas de regressão para avaliação dos modelos:

- **MSE** – Erro Quadrático Médio
- **MAE** – Erro Absoluto Médio
- **RMSE** – Raiz do Erro Quadrático Médio
- **MAPE** – Erro Percentual Absoluto Médio
- **R²** – Coeficiente de Determinação

---

## 🧪 Exemplo de Uso

Após treinar os modelos, é possível carregar qualquer um deles com `pickle` e realizar predições:

```python
import pickle

modelo = pickle.load(open("lgbm_model.pkl", "rb"))
predicoes = modelo.predict(X_test)

