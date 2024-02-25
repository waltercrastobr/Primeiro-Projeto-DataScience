# Primeiro Projeto Prático DataScience
Estou animado em compartilhar meu primeiro projeto prático em Ciência de Dados, feito na linguagem Python, focado na análise de Churn usando um dataset com 998 linhas e 12 colunas.

A análise de churn é a análise e previsão da taxa de cancelamento de clientes de um serviço ou produto ao longo do tempo. 

## [Etapa 1: Análise e Tratamento de Dados](https://github.com/waltercrastobr/Primeiro-Projeto-DataScience/blob/main/analise-tratamento-dados.ipynb)

-  Nesta etapa, explorei os dados e realizei os tratamentos necessários:
  - Utilizei as bibliotecas 'pandas' e 'statistics' para manipulação e análise dos dados
  - Renomeei as colunas que estavam no formato X1, X2, X3... para nomes mais descritivos
  - Removi valores nulos do dataset
  - Verifiquei e corrigi valores que estavam fora do domínio esperado em cada coluna.

## [Etapa 2: Criação de Modelos de Machine Learning](https://github.com/waltercrastobr/Primeiro-Projeto-DataScience/blob/main/modelos_machinelearning.ipynb)

-  Nesta etapa, realizei tratamentos adicionais nas colunas categóricas e construí quatro modelos de machine learning:

  - Utilizei a biblioteca 'sklearn' para importar os modelos, tratar colunas 'object' e calcular as métricas de acurácia.
  - Converti as colunas do tipo 'object' para o formato 'int', mais adequado para modelos de classificação.
  - Na coluna Gênero, transformei 'Masculino' e 'Feminino' em 'MasculinoCheck', atribuindo o valor 1 para masculino e 0 para feminino.
  - Na coluna Estado, utilizei o OneHotEncoder para transformar os dados 'RS', 'PR' e 'SC' em matrizes 'Estado_RS', 'Estado_PR' e 'Estado_SC', respectivamente, onde 0 --representa não pertencer ao estado e 1 pertencer ao estado.
  - Verifiquei e corrigi novos valores faltantes.
  - Escolhi três modelos de classificação: Árvores de Decisão, Regressão Logística e KNeighborsClassifier.
  - Realizei as métricas de acurácia para avaliação dos modelos.
  - Criei um dataframe para armazenar os valores de acurácia dos modelos.
  - As acurácias foram: Árvore de Classificação: 83%,  KNeighbors: 71,8%, Regressão Logística: 78,7%
    
## Etapa 3: Considerações finais

#### Motivos para a Escolha dos Modelos
Os modelos de regressão logística, árvore de decisão e k-Nearest Neighbors (k-NN) são frequentemente recomendados para análise de churn devido às suas características e capacidades específicas, que se alinham bem com os desafios desse tipo de análise.

1. *Regressão Logística*: É amplamente utilizada em problemas de classificação binária, como a previsão de churn. Produz resultados interpretáveis e não requer muitos ajustes de hiperparâmetros.

2. *Árvore de Decisão*: Pode capturar padrões complexos nos dados e é facilmente interpretável, ajudando a entender quais variáveis são mais importantes na decisão de churn.

3. *k-NN*: É um algoritmo simples e intuitivo que usa a proximidade dos vizinhos para fazer previsões. Pode ser útil na análise de churn para identificar clientes com comportamentos semelhantes. Não requer suposições sobre a distribuição dos dados e pode lidar com relações não-lineares, mas pode ser afetado por dados ruidosos e alta dimensionalidade.

Esses modelos são escolhas comuns devido à sua capacidade de lidar com diferentes tipos de dados e padrões, bem como à sua interpretabilidade.

#### Métricas de Avaliação
Em análises de churn, a ênfase é dada aos falsos negativos, pois é mais prejudicial errar ao prever que um cliente não vai cancelar o serviço quando na verdade ele vai. Portanto, é comum priorizar métricas que reduzam os falsos negativos, como o recall.

Ao comparar as matrizes de confusão dos modelos trabalhados, observamos que a Regressão Logística possui um menor número de falsos negativos (8) em relação aos verdadeiros positivos, quando comparada com os outros modelos. Isso sugere que ela pode ser mais adequada se a prioridade for minimizar a perda de clientes.

No entanto, é válido ressaltar que a escolha do modelo também deve levar em consideração outros fatores, como a interpretabilidade do modelo e o custo de implementação.

#### Conclusão
O projeto apresentou uma abordagem sólida para análise de churn, com tratamento adequado dos dados e escolha de modelos relevantes. A Regressão Logística se destacou por sua menor taxa de falsos negativos, mas a escolha do modelo ideal deve considerar o contexto específico da empresa e seus objetivos. Ressalta-se a experimentação diferentes modelos e técnicas de modelagem para encontrar a melhor solução para um determinado problema de churn.
    



