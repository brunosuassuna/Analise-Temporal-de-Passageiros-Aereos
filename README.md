# ✈️ Análise de Séries Temporais de Passageiros Aéreos

Este projeto apresenta uma análise de dados históricos de passageiros aéreos, utilizando técnicas de séries temporais com Python. O objetivo é entender os padrões históricos, identificar tendências e prever o número de passageiros para os próximos meses com o uso de modelos estatísticos.

## 📊 Objetivo

- Explorar a evolução do número de passageiros ao longo do tempo.
- Identificar tendências e sazonalidades.
- Realizar previsões com modelos de séries temporais.
- Visualizar insights relevantes por meio de gráficos.

## 📁 Dataset

O dataset utilizado é de domínio público e está disponível no repositório de datasets de John Brownlee:

- 📌 [airline-passengers.csv](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv)

Ele contém o número mensal de passageiros de uma companhia aérea internacional entre os anos de 1949 e 1960.

## 🔧 Tecnologias e Bibliotecas Utilizadas

- Python 3.x  
- pandas  
- matplotlib  
- statsmodels  

## 🧠 Metodologia

### 1. Carregamento dos Dados
Os dados foram carregados diretamente da web (formato CSV) com a biblioteca `pandas`.

### 2. Preparação
- Conversão da coluna de datas.
- Definição da coluna "Month" como índice da série temporal.

### 3. Análise Exploratória
- Visualização da série temporal com `matplotlib`.
- Observação de tendências e sazonalidade nos dados.

### 4. Decomposição
- Separação da série em três componentes: **Tendência**, **Sazonalidade** e **Resíduos** com o método `seasonal_decompose`.

### 5. Previsão com Holt-Winters
- Aplicação do modelo de **Suavização Exponencial** (Holt-Winters) para prever os 12 meses seguintes.
- Visualização dos resultados em gráfico.

### 6. Avaliação do Modelo
- Cálculo do Erro Médio Absoluto (MAE) para avaliar a acurácia da previsão.

## 📈 Resultados

- A série temporal apresenta um crescimento com forte padrão sazonal anual.
- O modelo Holt-Winters forneceu previsões coerentes com os padrões históricos observados.
- A previsão pode ser utilizada para planejamento e tomada de decisão estratégica.

## 📌 Conclusão

Este notebook demonstrou como realizar uma análise completa de séries temporais com Python, utilizando um dataset clássico. As técnicas aplicadas aqui podem ser facilmente adaptadas para dados reais de sensores IoT, financeiros, industriais, etc.

## 🚀 Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/analise-series-passageiros.git

## 📬 Contato

- **Email:** brunosuassuna.dev@gmail.com

- **LinkedIn:** www.linkedin.com/in/bruno-suassuna-698aa7235

**Licença:** [MIT](https://opensource.org/license/MIT)
