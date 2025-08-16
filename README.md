# 📊 Análise de Evasão de Clientes (Churn) - TelecomX 🎯

## 1. Propósito da Análise
Este projeto tem como objetivo analisar os dados de **churn (evasão de clientes)** da empresa fictícia TelecomX. Utilizando Python e bibliotecas de Data Science, a análise explora os dados para identificar os principais fatores que levam os clientes a cancelar seus serviços e, ao final, constrói um modelo de Machine Learning para prever esse comportamento.

Os principais objetivos são:
* Realizar uma análise exploratória (EDA) para extrair insights.
* Identificar os fatores que mais influenciam a evasão de clientes.
* Construir e avaliar um modelo preditivo para apoiar a tomada de decisões estratégicas de retenção.

---

## 📂 Estrutura do Projeto e Organização dos Arquivos
O projeto está organizado da seguinte forma para facilitar a compreensão e a reprodutibilidade:

* **`Telecom_Finalizado.ipynb`**: Notebook principal que contém todo o código e as etapas da análise, desde o carregamento e tratamento dos dados, passando pela visualização, modelagem e avaliação dos resultados.
* **`TelecomX_Data.json`**: Base de dados em formato JSON com as informações dos clientes, carregada diretamente de uma URL dentro do notebook.
* **`requirements.txt`**: Lista as dependências Python para que o ambiente de análise possa ser facilmente replicado.

---

## 📊 Exemplos de Gráficos e Insights Obtidos
Durante a análise, foram gerados diversos gráficos que revelaram padrões importantes sobre o churn.

📌 **Taxa de Churn por Tipo de Contrato**
* **Observação:** O gráfico de barras mostrou que clientes com **contrato mensal (Month-to-month)** possuem uma taxa de churn significativamente maior em comparação com clientes de contratos anuais ou bianuais.
* **Insight:** A falta de um compromisso de longo prazo torna esses clientes mais propensos a cancelar o serviço.

📌 **Análise de Correlação**
* **Observação:** A matriz de correlação (heatmap) indicou que variáveis como **tempo de permanência (tenure)** e **tipo de contrato (Contract)** têm uma correlação negativa forte com o churn, ou seja, quanto maiores os valores, menor a chance de evasão.
* **Insight:** Clientes mais antigos e com contratos longos são mais leais.

📌 **Importância das Variáveis (Feature Importance)**
* **Observação:** O modelo de Machine Learning (Random Forest) identificou que as variáveis mais importantes para prever o churn são, em ordem: **tempo de permanência (tenure)**, **tipo de contrato (Contract)**, **valor total da fatura (Charges.Total)** e **serviço de internet (InternetService)**.
* **Insight:** Focar em estratégias de retenção para clientes novos, com contratos mensais e que possuem apenas serviços básicos, pode gerar o maior impacto na redução do churn.

---
4.  **Inicie o Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
    Após iniciar, abra o arquivo `Telecom_Finalizado.ipynb` e execute as células.
