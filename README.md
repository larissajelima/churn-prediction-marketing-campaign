# 📊 Predição de Churn para Otimização de Campanhas de Marketing

🚀 **Notebook completo disponível no Colab:**  
👉 https://colab.research.google.com/drive/1Ex-zEG7KYSD0AbRQmDrE9TalJcRZ34YC?usp=sharing  

> 💡 Recomenda-se abrir o notebook no Colab para visualizar todas as etapas e resultados.

---

## 🚀 Resultado Principal

📈 Melhor estratégia: **Threshold = 0.1**  
💰 Estratégia mais lucrativa: abordagem **agressiva**  

➡️ O modelo com threshold mais baixo gerou maior lucro,  
pois o valor da venda compensa o custo de abordar clientes que não convertem.

---

## 🎯 Objetivo

Empresas que realizam campanhas de marketing enfrentam um desafio:

- cada contato com cliente tem custo  
- nem todos os clientes aceitam a oferta  

O objetivo deste projeto é prever quais clientes têm maior probabilidade de aceitar,
permitindo direcionar campanhas de forma mais eficiente e maximizar o lucro.

---

## 🧠 Estratégia de Negócio

Neste projeto, a decisão NÃO é baseada apenas em acurácia.

O foco é maximizar o retorno financeiro considerando:

- valor da venda  
- custo da campanha  
- erros do modelo (falsos positivos e falsos negativos)  

---

## ⚙️ Etapas do Projeto

### 1. Preparação dos Dados
- verificação de tipos e consistência  
- tratamento de variáveis categóricas (`get_dummies`)  
- remoção de variável com leakage (`duration`)  

---

### 2. Modelagem
- Decision Tree  
- comparação entre modelo padrão e com `class_weight='balanced'`  

---

### 3. Avaliação
- matriz de confusão  
- precision, recall e f1-score  

---

### 4. Otimização de Estratégia
- uso de probabilidades (`predict_proba`)  
- teste de diferentes thresholds  
- cálculo de lucro por estratégia  

---

## 📈 Resultados

- Modelo inicial: comportamento mais conservador  
- Perda significativa de clientes potenciais (alto falso negativo)  

Após ajuste:

- aumento do recall  
- redução de perdas de clientes  
- aumento do custo operacional (mais campanhas)  
- **lucro total maior**

---

## 💰 Lógica de Negócio

A decisão foi baseada na seguinte fórmula:
lucro = (TP * valor_venda) - ((TP + FP) * custo_campanha)

Onde:

- TP → clientes que aceitaram e foram corretamente previstos  
- FP → clientes abordados que não aceitaram  

---

## 🧠 Insight Principal

O melhor modelo não é o mais preciso.

👉 É o que gera mais valor para o negócio.

Ao reduzir o threshold, o modelo se torna mais agressivo,
capturando mais clientes com potencial de conversão.

Mesmo com maior custo de campanha, o retorno financeiro foi superior.

---

## 📊 Visualização

O gráfico de lucro por threshold mostra claramente que estratégias mais agressivas
geram maior retorno neste cenário.

---

## 🧠 Conclusão

Este projeto demonstra que:

- métricas tradicionais como acurácia nem sempre são suficientes  
- decisões devem ser guiadas por impacto financeiro  
- ajustes simples como threshold podem transformar a estratégia  

---

## 🗂️ Estrutura do Projeto
```
churn-prediction-marketing-campaign/
│
├── churn_marketing_profit_optimization.ipynb
└── README.md
```

---

## 👩‍💻 Autora

**Larissa Lima**  
📍 Brasil  
🎯 Transição para área de Dados / BI
