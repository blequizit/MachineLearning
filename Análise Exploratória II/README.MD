# 🚗 Análise Exploratória II - Preço de Carros

Este repositório contém um projeto de Análise Exploratória de Dados (EDA) aplicado a um conjunto de dados de preços de carros, com o objetivo de entender os fatores que influenciam no valor dos veículos.

## 🎯 Objetivo

Este projeto aplica técnicas de Análise Exploratória de Dados para compreender as características dos veículos e suas relações com o preço final. A análise busca identificar padrões, correlações e comportamentos relevantes que possam ser utilizados em modelos preditivos futuros.

## 📄 Descrição do Dataset

O dataset `CarPrice_Assignment.csv` contém informações técnicas e comerciais de automóveis. Abaixo está o dicionário de dados:

- `Car_ID`: Identificador único
- `Symboling`: Classificação de risco de seguro
- `carCompany`: Marca do carro
- `fueltype`: Tipo de combustível
- `aspiration`: Tipo de aspiração do motor
- `doornumber`: Número de portas
- `carbody`: Tipo de carroceria
- `drivewheel`: Tipo de tração
- `enginelocation`: Localização do motor
- `wheelbase`, `carlength`, `carwidth`, `carheight`: Dimensões do veículo
- `curbweight`: Peso do veículo
- `enginetype`: Tipo de motor
- `cylindernumber`: Número de cilindros
- `enginesize`: Tamanho do motor
- `fuelsystem`: Sistema de combustível
- `boreratio`, `stroke`, `compressionratio`: Especificações internas do motor
- `horsepower`: Potência do motor
- `peakrpm`: Rotação máxima
- `citympg`, `highwaympg`: Consumo na cidade/estrada
- `price`: Preço final do carro (variável dependente)

## 🛠️ Bibliotecas Utilizadas

- `pandas`
- `numpy`
- `plotly.express`
- `plotly.graph_objects`
- `seaborn`
- `matplotlib`

## 📊 Etapas Realizadas

### 📌 Leitura e Limpeza de Dados

- Leitura com `pandas`
- Estatísticas descritivas com `df.describe()`
- Detecção de dados ausentes e valores duplicados

### 📌 Análise Univariada

- Distribuição da variável `price`
- Distribuições de variáveis categóricas com histogramas

### 📌 Análise de Correlação

- Geração de matriz de correlação
- Visualização com `px.imshow`

### 📌 Análise Bivariada

- Relação entre `enginesize` e `price`
- Boxplots entre `price` e variáveis como `carbody`, `fueltype`, `aspiration`, `drivewheel`, `cylindernumber`
- Médias de preço por categoria com gráficos de barra

### 📌 Análise de Consumo (citympg)

- Relações entre `enginesize`, `horsepower`, `curbweight` e `citympg`
- Boxplots e scatterplots de consumo por tipo de tração e número de cilindros

## 📁 Estrutura do Projeto

- `Analise Descritiva.ipynb`: Notebook com toda a análise exploratória
- `CarPrice_Assignment.csv`: Base de dados analisada
- `README.md`: Arquivo atual com detalhes do projeto

## 💡 Conclusões Iniciais

A análise revelou diversas relações esperadas, como o aumento do preço com o aumento do tamanho do motor, potência, peso e número de cilindros. Carros com aspiração "turbo" ou tração diferenciada também apresentam variações no preço e consumo.

## 👨‍💻 Autor

**Eduardo Ferreira**  
📧 eduds1010@gmail.com  
🔗 [github.com/blequizit](https://github.com/blequizit)

## 🙏 Agradecimentos

Agradecimento ao professor **Leandro Romualdo da Silva**, cujas aulas foram fundamentais para a construção deste projeto.
