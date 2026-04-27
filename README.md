# 📊 Desafio 01 — Análise Estatística e Seleção de Variáveis (SDM)

## 🎯 Objetivo

Analisar estatisticamente um conjunto de dados de presença/ausência (ou pseudo-ausência) de *Brassica napus* e propor um conjunto final de variáveis para uso em um modelo de distribuição de espécies (SDM).

O foco principal é investigar e tratar **colinearidade entre variáveis** utilizando:
- Matriz de correlação
- VIF (Variance Inflation Factor)
- vifstep
- vifcor

---

## 📂 Dados

O dataset contém:
- Coordenadas geográficas
- Informações temporais
- Variáveis ambientais e climáticas
- Variável resposta (presença/ausência)

---

## 🔍 Etapas da Análise

### 1. Análise Exploratória
- Estatísticas descritivas
- Distribuição das variáveis
- Identificação de outliers

---

### 2. Tratamento de Valores Ausentes
- Identificação de NA/Null
- Estratégias:
  - Remoção
  - Imputação (quando aplicável)

---

### 3. Matriz de Correlação
- Correlação de Pearson (ou Spearman)
- Identificação de variáveis altamente correlacionadas

Critério utilizado:
- |r| > 0.7 → alta correlação

---

### 4. Análise de Multicolinearidade (VIF)

- Cálculo do VIF para cada variável
- Critério:
  - VIF > 5 ou 10 → variável problemática

---

### 5. Seleção de Variáveis

#### 🔹 vifstep
- Remove iterativamente variáveis com maior VIF
- Mais robusto e controlado

#### 🔹 vifcor
- Remove variáveis com base na correlação entre pares
- Mais rápido, porém mais agressivo

---

## ✅ Resultado Esperado

- Conjunto final de variáveis:
  - Baixa colinearidade
  - Alta relevância ecológica
  - Boa interpretabilidade

---

## 🌱 Justificativa

### Estatística
- Redução de multicolinearidade
- Maior estabilidade do modelo
- Evita overfitting

### Ecológica / Agronômica
- Variáveis com impacto direto na distribuição da espécie
- Relevância climática e ambiental

---

## 📈 Impacto no Modelo SDM

- Melhor performance preditiva
- Maior generalização
- Melhor interpretação dos resultados

---

## 📄 Entregável

Relatório técnico contendo:
- Resumo dos dados
- Problemas encontrados
- Análise de valores ausentes
- Matriz de correlação
- VIF
- Comparação vifstep vs vifcor
- Variáveis finais
- Justificativa
- Impacto no modelo

---

## 🛠️ Tecnologias Sugeridas

- Python (pandas, numpy, statsmodels)
- ou R (dplyr, usdm, caret)

---

Contato em email: siapesq@gmail.com

## 🚀 Autor

Desafio técnico — etapa de análise estatística
