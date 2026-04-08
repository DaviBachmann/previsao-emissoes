# 📊 Previsão de Emissões de Documentos Fiscais

## 🎯 Objetivo

Desenvolver um modelo preditivo capaz de estimar o volume mensal de emissões de documentos fiscais de um cliente, com o objetivo de apoiar decisões de negócio como planejamento financeiro e dimensionamento de infraestrutura.

---

## 🧠 Problema de Negócio

Empresas que lidam com alto volume de emissão de documentos precisam antecipar demandas para:

- evitar sobrecarga de sistemas
- planejar custos operacionais
- melhorar a previsibilidade financeira

Este projeto busca resolver esse problema utilizando dados históricos.

---

## 🔍 Etapas do Projeto

- Coleta e tratamento dos dados
- Análise exploratória (EDA)
- Engenharia de features
- Treinamento de modelos
- Validação e análise de desempenho

---

## ⚙️ Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## 🧩 Engenharia de Features

Foram criadas variáveis baseadas no comportamento temporal dos dados:

- Média móvel (2, 3 e 4 meses)
- Emissões do mês anterior (lag)
- Crescimento e aceleração de crescimento
- Máximo recente
- Transformação logarítmica

Um ponto crítico foi evitar **data leakage**, garantindo que todas as variáveis utilizassem apenas informações passadas.

---

## 🤖 Modelos Testados

- Regressão Linear
- Random Forest

A regressão linear apresentou melhor desempenho para o problema.

---

## 📈 Resultados

- **MAPE:** ~10.58%
- **MAE:** ~1.7M
- **RMSE:** ~2.1M

O modelo demonstrou boa capacidade de previsão considerando a quantidade limitada de dados.

---

## 💡 Principais Insights

- Engenharia de features teve maior impacto que a escolha do modelo
- Modelos simples podem performar melhor com poucos dados
- Evitar data leakage é essencial para garantir confiabilidade

---

## 🚀 Possíveis Evoluções

- Inclusão de mais dados históricos
- Modelos específicos por cliente
- Uso de modelos de séries temporais
- Integração com dashboards (Power BI)

---

## 📌 Conclusão

O projeto demonstra como dados históricos podem ser utilizados para gerar previsões confiáveis e apoiar decisões estratégicas.

---

## 📎 Como executar

```bash
pip install -r requirements.txt
