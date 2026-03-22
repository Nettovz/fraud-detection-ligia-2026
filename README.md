# Detecção de Fraudes em Transações Financeiras

Autor: Deoclécio Ivo de Melo Netto  
Trilha: Aprendizado de Máquina  

---

## Objetivo

Desenvolver uma solução de classificação binária para identificar transações fraudulentas em um cenário de forte desbalanceamento entre classes.

A avaliação competitiva foi realizada com base na métrica **ROC-AUC**, conforme especificado no desafio da plataforma Kaggle.

---

## Modelos Avaliados

- Regressão Logística
- LightGBM (Gradient Boosting Decision Trees)

Foram aplicadas estratégias para lidar com o desbalanceamento, incluindo:

- `class_weight="balanced"`
- Ajuste de threshold com base na curva Precision-Recall
- Maximização do F1-score
- Análise de matriz de confusão

---

## Metodologia

1. Análise exploratória dos dados
2. Divisão estratificada em treino e validação
3. Treinamento dos modelos
4. Ajuste estratégico do threshold
5. Avaliação via ROC-AUC, Recall, Precision e F1-score

---

## Resultados

Ambos os modelos apresentaram ROC-AUC próximo de 97%, com o LightGBM apresentando leve melhoria na redução de falsos positivos e falsos negativos.

---

fraud-detection-liga-2026/
│
├── notebook/
│   └── fraud_detection.ipynb
│
├── submissions/
│   ├── submission_LightGBM.csv
│   └── submission_logisticregression.csv
│
├── docs/
│   └── Fraud_Detection.pdf
│
├── requirements.txt
└── README.md
---

## Como Executar

1. Instalar as dependências:



2. Executar o notebook:

Abra o arquivo `fraud_detection.ipynb` em um ambiente Jupyter Notebook ou VSCode e execute as células sequencialmente.

### Ambiente recomendado

Python 3.10+

---

## Dataset

O dataset utilizado está disponível na competição oficial do Kaggle.  
Devido às regras de redistribuição da plataforma, os arquivos não estão incluídos neste repositório.

---

## Relatório Técnico

O relatório completo está disponível no arquivo:

`Fraud_Detection.pdf`

---

## Considerações

A solução busca equilibrar desempenho preditivo e interpretabilidade, analisando o impacto operacional dos erros de classificação em ambientes financeiros e demonstrando controle experimental e validação consistente.


