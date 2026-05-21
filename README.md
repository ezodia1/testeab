# Análise de Teste A/B: Sistema de Recomendações

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Statsmodels](https://img.shields.io/badge/Statsmodels-ADADAD?style=for-the-badge)

## 📌 Visão Geral do Projeto
Este projeto analisa os resultados de um teste A/B realizado por uma loja virtual internacional. O objetivo foi avaliar se a introdução de um novo sistema de recomendações impactaria positivamente a conversão dos usuários ao longo do funil de compra, utilizando testes de hipóteses estatísticas.

## 🎯 Objetivos de Negócio
* **Análise do Funil:** Mapear e comparar as taxas de conversão nas etapas `product_page → product_cart → purchase` entre os grupos de controle e teste.
* **Validação do Experimento:** Verificar a integridade dos dados e identificar possíveis contaminações no experimento.
* **Tomada de Decisão Baseada em Dados:** Recomendar a implementação ou descarte do novo sistema com base na significância estatística.

## 🛠️ Stack Técnica
* **Linguagem:** Python
* **Manipulação de Dados:** Pandas, NumPy
* **Visualização:** Matplotlib
* **Estatística:** Statsmodels (Teste Z para proporções)

## 📉 Metodologia
1. **Preparação de Dados:** Limpeza, conversão de tipos, remoção de usuários presentes em ambos os grupos e filtragem para a região EU.
2. **Análise Exploratória (EDA):** Distribuição de eventos ao longo dos dias, média de eventos por usuário por grupo e identificação de campanhas de marketing ativas durante o período do teste.
3. **Análise do Funil:** Cálculo das taxas de conversão por grupo em cada etapa, com visualização comparativa.
4. **Testes Estatísticos:** Teste Z para proporções nas etapas `product_cart` e `purchase`, com nível de significância de 0.05.

## 🏆 Resultados e Conclusões
* **Desempenho do Novo Sistema:** Em ambas as etapas testadas, o p-value foi superior a 0.05, indicando que a diferença de ~3.58% entre os grupos não é estatisticamente significativa.
* **Meta não atingida:** O experimento exigia aumento mínimo de 10% em cada etapa — o resultado ficou bem abaixo disso.
* **Limitações identificadas:** Grupos desbalanceados (A=1939 vs B=655), número de participantes abaixo do previsto (2594 vs 6000 esperados) e campanha de marketing ativa durante o período do teste.
* **Recomendação Final:** Não implementar o novo sistema de recomendações. Recomenda-se redesenhar o experimento com grupos balanceados e fora de períodos de campanhas de marketing.

---

### 📂 Estrutura do Repositório
* `teste_ab.ipynb`: Notebook Jupyter contendo toda a análise, códigos e visualizações.
* `data/`: Pasta contendo os arquivos de dados utilizados na análise.

---
**Enzo Bombassaro de Freitas** | *Data Analyst* | [LinkedIn](https://www.linkedin.com/in/enzo-bombassaro/) | [GitHub](https://github.com/ezodia1)

