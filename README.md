# Previsão de Preços de Ações da Apple (AAPL) com Machine Learning

## Introdução
Este projeto utiliza dados históricos de preços de ações da Apple (AAPL) para construir um modelo de Machine Learning capaz de prever os preços de fechamento das ações. O projeto abrange desde a coleta e preparação dos dados até a construção, treinamento, avaliação e visualização dos resultados do modelo.

## Estrutura do Projeto
1. **Coleta e Preparação dos Dados**
2. **Análise Exploratória de Dados (EDA)**
3. **Feature Engineering**
4. **Divisão dos Dados em Treinamento e Teste**
5. **Construção e Treinamento do Modelo**
6. **Avaliação do Modelo**
7. **Visualização dos Resultados**

## Requisitos
- Python 3.7+
- Pandas
- NumPy
- yfinance
- Matplotlib
- Seaborn
- scikit-learn
- Plotly

## Instalação
Clone este repositório e instale os pacotes necessários:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
pip install -r requirements.txt

##Uso
Execute o notebook previsao_precos_acoes.ipynb no Google Colab ou em sua máquina local para reproduzir os resultados.

Coleta e Preparação dos Dados
Baixamos os dados históricos de preços de ações da Apple usando a biblioteca yfinance.

python
Copiar código
import pandas as pd
import yfinance as yf

ticker = 'AAPL'
data = yf.download(ticker, start='2010-01-01', end='2023-01-01')
data.head()
