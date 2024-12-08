# Projeto-2-Ada

# **Análise de Dados: Desempenho de Estudantes e Aprovação de Crédito**

Este projeto realiza análises exploratórias, clustering e modelagem preditiva em dois conjuntos de dados distintos: um sobre o desempenho de estudantes e outro sobre aprovação de crédito. Abaixo estão os detalhes sobre os datasets, métodos utilizados e os principais insights obtidos.

---

## **Dataset 1: Desempenho de Estudantes**

### **Descrição**
O conjunto de dados contém informações sobre estudantes e seus desempenhos acadêmicos em três disciplinas: matemática, leitura e escrita. Também inclui variáveis demográficas e socioeconômicas, como nível educacional dos pais e participação em cursos preparatórios.

### **Objetivos**
1. Analisar o impacto de fatores socioeconômicos no desempenho acadêmico.
2. Identificar grupos de estudantes com base nas notas.
3. Construir um modelo para prever o desempenho com base nas características dos estudantes.

### **Resultados**
- **Distribuição de Pontuações**:
  - A maioria dos estudantes obteve pontuações médias entre 70 e 80.
  - Leitura e escrita têm alta correlação (acima de 0.8).
- **Clusterização**:
  - Três grupos foram identificados pelo algoritmo KMeans, diferenciando estudantes com desempenho baixo, médio e alto.
  - O DBSCAN identificou um único cluster, indicando baixa variabilidade estrutural nos dados.
- **Modelo Supervisionado (Random Forest)**:
  - O modelo alcançou uma precisão de 99%, demonstrando alta capacidade preditiva.

### **Aplicação**
Os insights podem ser utilizados para:
- Desenvolver políticas educacionais mais inclusivas.
- Fornecer suporte adicional para grupos com baixo desempenho.
- Avaliar a eficácia de cursos preparatórios.

---

## **Dataset 2: Aprovação de Crédito**

### **Descrição**
Este conjunto de dados contém informações demográficas e financeiras sobre solicitantes de crédito, incluindo idade, renda, dívidas e histórico financeiro. A variável alvo indica se o crédito foi aprovado ou não.

### **Objetivos**
1. Explorar os fatores que influenciam a aprovação de crédito.
2. Identificar padrões e outliers no perfil dos solicitantes.
3. Construir um modelo para prever a aprovação de crédito.

### **Resultados**
- **Distribuição de Variáveis**:
  - A maioria dos solicitantes tem renda muito baixa (abaixo de 1.000).
  - Tempo de emprego está positivamente correlacionado com a aprovação.
- **Clusterização**:
  - KMeans identificou três clusters, com um grupo principal representando o perfil padrão.
  - DBSCAN destacou um pequeno grupo de outliers (13 indivíduos com características atípicas).
- **Modelo Supervisionado (Random Forest)**:
  - O modelo atingiu uma precisão de 73%, capturando padrões razoáveis na aprovação de crédito.

### **Aplicação**
Os insights podem ajudar instituições financeiras a:
- Ajustar políticas de crédito para diferentes perfis de risco.
- Oferecer produtos financeiros personalizados para perfis de alto risco.
- Melhorar a experiência de aprovação para clientes com características desfavoráveis.

---

## **Tecnologias e Bibliotecas Utilizadas**
- **Linguagem**: Python
- **Bibliotecas**:
  - `pandas`, `numpy` - Manipulação e análise de dados.
  - `matplotlib`, `seaborn` - Visualização de dados.
  - `sklearn` - Modelagem supervisionada e não supervisionada.

---

