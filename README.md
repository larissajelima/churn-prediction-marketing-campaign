# 📊 Predição de Churn em Campanha de Marketing

---

## 🚀 Resultado Principal

📈 Melhor estratégia: Threshold = 0.1  
💰 Maior lucro obtido: (coloca um número real seu)  

➡️ Estratégia agressiva se mostrou mais eficiente,
pois o valor da venda supera o custo da campanha.

---

## 🎯 Objetivo

Uma empresa realiza campanhas de marketing para oferecer um produto.
Cada contato tem um custo, e nem todos os clientes aceitam a oferta.

O objetivo deste projeto é prever quais clientes têm maior probabilidade de aceitar,
permitindo otimizar a campanha e maximizar o lucro.

---

## 🧠 Problema de Negócio

Sem modelo:
a empresa impactaria todos os clientes → alto custo

Com modelo:
é possível focar apenas nos clientes com maior probabilidade de conversão
---

## 📊 Decisão de Negócio

Nem sempre o modelo com maior acurácia gera mais lucro.

Neste projeto, a decisão é baseada no retorno financeiro considerando:

- valor da venda
- custo da campanha
- previsões do modelo

---

## 📈 Resultados

- Melhor threshold: **0.1**
- Estratégia: **agressiva**
- Recall alto (captura a maioria dos clientes que aceitariam)
- Maior lucro obtido no cenário analisado

---

## 📌 Principais Insights

O modelo inicial apresentou desempenho equilibrado,
mas com perda significativa de clientes potenciais.

Ao ajustar o threshold e priorizar recall,
foi possível aumentar o lucro da campanha,
mesmo com maior custo operacional.

Isso demonstra que decisões baseadas em métricas de negócio
são mais relevantes do que métricas tradicionais como acurácia.

---

## ⚙️ Etapas do Projeto

🔹 1. Carregamento dos Dados  

🔹 2. Limpeza e Preparação  
- remoção de variável com leakage (`duration`)  
- encoding de variáveis categóricas (`get_dummies`)  

🔹 3. Modelagem  
- Decision Tree  
- comparação entre modelo padrão e com `class_weight='balanced'`  

🔹 4. Avaliação  
- matriz de confusão  
- precision, recall e f1-score  

🔹 5. Otimização de Estratégia  
- ajuste de threshold  
- cálculo de lucro baseado em TP e FP  

🔹 6. Resultado Final  
- escolha do threshold com maior retorno financeiro  

---

## 🧠 Conclusão

Este projeto demonstra que a escolha do modelo não deve ser baseada apenas em acurácia,
mas sim no impacto financeiro da decisão.

Ao ajustar o threshold, foi possível transformar um modelo comum
em uma estratégia mais lucrativa para o negócio.

---

## 🗂️ Estrutura do Projeto

```text
churn-prediction-marketing-campaign/
│
├── notebook.ipynb
└── README.md

## 👩‍💻 Autor

**Larissa Lima**
📍 Brasil
🎯 Em transição para Analista de BI

---
