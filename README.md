# Primeiro Projeto Prático DataScience
Estou animado em compartilhar meu primeiro projeto prático em Ciência de Dados, focado na análise de Churn usando um dataset com 998 linhas e 12 colunas.

A análise de churn é a análise e previsão da taxa de cancelamento de clientes de um serviço ou produto ao longo do tempo. 

## [Etapa 1: Análise e Tratamento de Dados](https://github.com/waltercrastobr/Primeiro-Projeto-DataScience/blob/main/analise-tratamento-dados.ipynb)

-  Nesta etapa, explorei os dados e realizei os tratamentos necessários:
  - Utilizei as bibliotecas 'pandas' e 'statistics' para manipulação e análise dos dados
  - Renomeei as colunas que estavam no formato X1, X2, X3... para nomes mais descritivos
  - Removi valores nulos do dataset
  - Verifiquei e corrigi valores que estavam fora do domínio esperado em cada coluna.

## [Etapa 2: Criação de Modelos de Machine Learning](https://github.com/waltercrastobr/Primeiro-Projeto-DataScience/blob/main/modelos_machinelearning-Copy1.ipynb)

-  Nesta etapa, realizei tratamentos adicionais nas colunas categóricas e construí quatro modelos de machine learning:

  - Utilizei a biblioteca 'sklearn' para importar os modelos, tratar colunas 'object' e calcular as métricas de acurácia.
  - Converti as colunas do tipo 'object' para o formato 'int', mais adequado para modelos de classificação.
  - Na coluna Gênero, transformei 'Masculino' e 'Feminino' em 'MasculinoCheck', atribuindo o valor 1 para masculino e 0 para feminino.
  - Na coluna Estado, utilizei o OneHotEncoder para transformar os dados 'RS', 'PR' e 'SC' em matrizes 'Estado_RS', 'Estado_PR' e 'Estado_SC', respectivamente, onde 0 --representa não pertencer ao estado e 1 pertencer ao estado.
  - Verifiquei e corrigi novos valores faltantes.
  - Escolhi três modelos de classificação: Árvores de Decisão, Regressão Logística e KNeighborsClassifier.
  - Realizei as métricas de acurácia para avaliação dos modelos.
  - Criei um dataframe para armazenar os valores de acurácia dos modelos.



