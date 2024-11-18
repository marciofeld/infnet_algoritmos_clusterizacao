# Algoritmos de Inteligência Artificial para Clustericação [24E4_2]

## PROJETO DA DISCIPLINA - ENTREGA FINAL

## Aluno: Marcio Feldmann

Este projeto é uma análise de clusterização de países baseada em indicadores socioeconômicos. Foram utilizamos diferentes algoritmos de agrupamento, como **K-Means**, **Clusterização Hierárquica** e **K-Medoids**, para identificar padrões e semelhanças entre os países.

## **Objetivo**
O objetivo deste projeto é agrupar países em grupos semelhantes usando algoritmos de aprendizado não supervisionado. A análise ajuda a compreender como diferentes indicadores influenciam os agrupamentos e como tratar outliers nos dados.

---

## **Etapas do Projeto**

### **1. Importação de Bibliotecas e Dados**
- Foram utilizadas bibliotecas como `pandas`, `numpy`, `matplotlib` e `sklearn` para manipulação de dados, visualizações e clusterização.
- Os dados foram carregados de um arquivo CSV contendo indicadores como mortalidade infantil, expectativa de vida, PIB, entre outros, de acordo com o link fornecido pelo professor.

### **2. Pré-Processamento**
- **Normalização dos Dados**:
  - As variáveis numéricas foram escalonadas para o intervalo [0, 1] usando `MinMaxScaler`.
- **Tratamento de Outliers**:
  - Foi analisada a influência de valores extremos nos agrupamentos.

### **3. Aplicação de Algoritmos de Clusterização**
- **K-Means**:
  - Agrupou os países em 3 clusters de forma imperativa (a quantidade de clusters foi especificada manualmente).
  - É sensível a outliers devido ao uso de centróides baseados na média.
- **K-Medoids**:
  - Ajustado para usar medóides, tornando-o mais resistente a outliers.

### **4. Interpretação dos Resultados**
- Foi analisada a distribuição de indicadores dentro de cada cluster.
- Foram identificados os países que melhor representam cada cluster.
- Foi realizada a comparação dos resultados entre os algoritmos.

### **5. Visualização**
- Gráficos foram utilizados para explorar a faixa dinâmica dos dados.
- Um dendograma foi gerado para visualizar a clusterização hierárquica.

---

## **Principais Resultados**
- O **K-Means** agrupou os países de forma eficiente, mas apresentou sensibilidade a outliers.
- O **K-Medoids** melhorou a robustez ao lidar com valores extremos, mas teve maior custo computacional.

---

## **Fontes de Dados**
Os dados utilizados foram fornecidos em formato CSV através do arquivo `Country-data.csv` obtido [neste link](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data) e incluem indicadores globais.

---

## **Arquivos Gerados**
Durante a execução do Jupyter Notebook, os seguintes arquivos foram gerados para facilitar a posterior análise de comparação de clusters K-Médias e Clusterização Hierárquica
- `parte3_exercicio4_comparacao_clusters.csv`
- `parte3_exercicio4_justificacao_diferencas_clusters.csv`

---

## **Referências**
- [Scikit-Learn Documentation](https://scikit-learn.org/stable/)
- [K-Medoids Clustering](https://en.wikipedia.org/wiki/K-medoids)
- [Sensibilidade do K-Médias](https://scikit-learn.org/stable/modules/clustering.html#k-means)
- [Comparação K-Médias e K-Medoids](https://www.geeksforgeeks.org/k-means-vs-k-medoids-clustering/)
- [Lidando com Outliers](https://www.datageeks.com.br/outliers/)
- [Robustez do DBSCAN](https://scikit-learn.org/stable/modules/clustering.html#dbscan)
- [Comparação entre DBSCAN e K-Means](https://towardsdatascience.com/dbscan-clustering-explained-97556a2ad556)

---
