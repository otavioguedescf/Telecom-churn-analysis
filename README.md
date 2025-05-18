# Telecom Churn Analysis

Este repositório apresenta uma análise completa sobre o churn de clientes em uma empresa de telecomunicações, desenvolvida como parte de um case de entrevista. O projeto utiliza Python para tratar os dados, aplicar análise exploratória e empregar classificação zero-shot com LLMs (Large Language Models).

---

## 🌐 Objetivo
A empresa de telecomunicações contratou a A3Data para avaliar o cenário de churn elevado dos seus clientes. Como o produto possui um alto custo de instalação (setup), a empresa busca estratégias para reduzir esse churn. Este projeto visa identificar padrões de comportamento, fatores críticos e propor recomendações com base nos dados.

---

## 📂 Estrutura do Projeto

### ▪️ 1. Importações e Configuração Inicial
- 1.1 Importação das bibliotecas  
- 1.2 Configurações de ambiente (pandas, warnings, seed, etc.)

### ▪️ 2. Carregamento e Pré-Tratamento dos Dados
- 2.1 Leitura do arquivo `.csv`  
- 2.2 Visão geral com `.info()`, `.head()` e `.describe()`  
- 2.3 Conversão de colunas de data  
- 2.4 Criação da variável `Churn`  
- 2.5 Cálculo do tempo de contrato (em meses)  
- 2.6 Tratamento de valores ausentes  

### ▪️ 3. Engenharia de Variáveis
- 3.1 `Reclamacoes_por_mes`  
- 3.2 Faixa etária  
- 3.3 Flag para produto isolado x pacote  

### ▪️ 4. Análise Exploratória Macro (Visão de Negócio)
- 4.1 Entrada e saída de clientes por ano  
- 4.2 Evolução do faturamento  
- 4.3 Vendas por tipo de serviço  
- 4.4 Ticket médio geral e por serviço  

### ▪️ 5. NLP com LLM (Zero-Shot Classification)
- 5.1 Limpeza da coluna de comentários  
- 5.2 Carregamento do modelo `facebook/bart-large-mnli`  
- 5.3 Definição das categorias: elogio, reclamação, sugestão...  
- 5.4 Classificação zero-shot  
- 5.5 Geração da coluna `categoria_reclamacao`  

### ▪️ 6. Análise Exploratória Micro
- 6.1 Número de reclamações totais  
- 6.2 Perfil sociodemográfico das reclamações  
- 6.3 Reclamações por localização  
- 6.4 Produto isolado vs pacote  
- 6.5 Ticket médio e estratégia de pacotes  

### ▪️ 7. Salvamento do DataFrame final

---

## 🔹 Resultados e Insights
Os principais resultados estão consolidados na apresentação (PowerPoint) entregue junto ao case. A análise exploratória revelou padrões importantes de churn associados a tempo de contrato, tipo de serviço, perfil do cliente e reclamações. A classificação automática de comentários via LLM permitiu identificar feedbacks críticos de forma escalável.

---

## 🏃‍♂️ Como Executar

1. Abra as pasta "noteobook", baixe o arquivo .ipynb e execute  em Jupyter, VSCode ou Colab
