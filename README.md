# 📊 Predição de Churn em Campanha de Marketing

---

## 🎯 Objetivo

Uma empresa faz campanhas de marketing para oferecer um produto.
O custo de contato existe, e nem todos os clientes aceitam.

O objetivo é usar dados para prever quais clientes têm maior chance de aceitar,
e assim maximizar o lucro da campanha.

---

## 📊 Decisão de Negócio

Nem todo modelo com maior acurácia gera mais lucro.
A decisão será baseada no retorno financeiro considerando:

- valor da venda
- custo da campanha
- taxa de acerto do modelo

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
🔹 2. Limpeza e preparação dos dados
- limpeza
- remoção de duration (leakage)
- encoding (get_dummies)
🔹 2. Modelagem
- Decision Tree
- versão normal vs balanced
🔹 3. Avaliação
- matriz de confusão
- precision / recall
🔹 4. Ajuste de estratégia
- uso de threshold
- análise de lucro
🔹 5. Resultado final

---

## 🗂️ Estrutura do Projeto

```text
churn-prediction-marketing-campaigns/
│
├── data/
│   └── raw/
│       ├── import_kaggle.py
│       └── load_data.py
│
├── insights/
│   └── principais_insights.md
│
├── python/
│   ├── limpeza.py
│   ├── preparacao.py
│   ├── modelo.py
│   ├── avaliação.py
│   └── threshold_lucro.py
│
└── README.md
```

---

## 👩‍💻 Autor

**Larissa Lima**
📍 Brasil
🎯 Em transição para Analista de BI

---
