# ✈️ Análise de Séries Temporais: Passageiros Aéreos

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat-square&logo=python)

Este projeto apresenta uma análise aprofundada de séries temporais sobre o número mensal de passageiros aéreos de 1949 a 1960. Utilizando bibliotecas do ecossistema Python, o estudo visa identificar padrões históricos, compreender tendências e realizar previsões com modelos estatísticos clássicos.

---

## 📌 Sumário

- [🎯 Objetivo](#-objetivo)
- [📁 Fonte dos Dados](#-fonte-dos-dados)
- [🧰 Tecnologias e Bibliotecas](#-tecnologias-e-bibliotecas)
- [🧠 Metodologia Aplicada](#-metodologia-aplicada)
- [📊 Resultados e Insights](#-resultados-e-insights)
- [📈 Conclusões](#-conclusões)
- [🚀 Como Executar](#-como-executar)
- [📜 Licença](#-licença)
- [✉️ Contato](#-contato)

---

## 🎯 Objetivo

- 📈 Analisar a evolução do número de passageiros ao longo dos anos.
- 🔍 Detectar tendências e padrões sazonais.
- 🤖 Construir um modelo de previsão usando Holt-Winters.
- 📊 Visualizar os resultados por meio de gráficos informativos.

---

## 📁 Fonte dos Dados

O dataset é público e foi disponibilizado por John Brownlee:

📄 [airline-passengers.csv](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv)

- Período: Jan/1949 a Dez/1960  
- Frequência: Mensal  
- Atributo principal: Número de passageiros por mês

---

## 🧰 Tecnologias e Bibliotecas

| Biblioteca      | Finalidade                                |
|-----------------|--------------------------------------------|
| `pandas`        | Manipulação e limpeza de dados             |
| `matplotlib`    | Visualização de séries temporais           |
| `statsmodels`   | Modelagem estatística e decomposição       |
| `numpy`         | Operações numéricas básicas (se necessário) |
| `seaborn`       | Visualização complementar (opcional)       |

---

## 🧠 Metodologia Aplicada

### ✅ 1. Carregamento dos Dados
- Leitura direta do CSV via URL com `pandas`.

### 🔧 2. Pré-processamento
- Conversão da coluna `"Month"` para `datetime`.
- Definição como índice para formar a série temporal.

### 📊 3. Análise Exploratória
- Gráficos de linha para identificar padrões visuais.
- Avaliação visual de tendência e sazonalidade.

### 📉 4. Decomposição de Série
- Utilização do método `seasonal_decompose` para extrair:
  - Tendência
  - Sazonalidade
  - Ruído

### 🔮 5. Modelagem Preditiva com Holt-Winters
- Aplicação da Suavização Exponencial com componente aditivo.
- Previsão dos 12 meses subsequentes.

### 📏 6. Avaliação de Desempenho
- Cálculo do MAE (Mean Absolute Error) para medir acurácia.

---

## 📊 Resultados e Insights

- A série apresenta crescimento linear com sazonalidade anual clara.
- A decomposição confirmou ciclos previsíveis e aumento consistente no número de passageiros.
- O modelo Holt-Winters foi eficaz para reproduzir os padrões históricos e projetar estimativas confiáveis.

---

## 📈 Conclusões

Este estudo demonstrou como aplicar técnicas estatísticas clássicas para análise e previsão de séries temporais. A metodologia pode ser facilmente adaptada a outros domínios, como:

- Tráfego de rede
- Vendas mensais
- Produção industrial
- Dados meteorológicos

---

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/brunosuassuna/Analise-Temporal-de-Passageiros-Aereos

2. Instale as dependências:
pip install -r requirements.txt
```

## ✉️ Contato
- **Email:** brunosuassuna.dev@gmail.com
- **LinkedIn:** www.linkedin.com/in/brunosuassuna

