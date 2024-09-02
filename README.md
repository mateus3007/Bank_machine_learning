# Bank_machine_learning
Este projeto realiza uma análise e modelagem de dados utilizando um conjunto de dados bancários, com o objetivo de preparar os dados para análise e aplicar técnicas de machine learning para previsão e clusterização. O fluxo de trabalho inclui:

Carregamento e Preparação dos Dados:

O conjunto de dados bank-data.csv é carregado usando a biblioteca pandas.
O código verifica a existência de várias colunas categóricas e as transforma em valores numéricos. Isso inclui as colunas sex, married, car, save_act, current_act, mortgage, pep, e region.
O ID da coluna é removido, e uma nova coluna percapita é criada para representar a renda per capita ajustada com base no estado civil dos clientes.
Análise Exploratória dos Dados:

O código exibe as primeiras linhas do DataFrame após cada transformação para verificar as mudanças.
Histogramas das variáveis são gerados para observar a distribuição dos dados.
Pré-processamento dos Dados:

Os dados são escalados usando StandardScaler para padronização.
Uma análise de cluster é realizada utilizando o algoritmo KMeans com 3 clusters, e os resultados são visualizados em um gráfico de dispersão.
Modelagem e Avaliação:

Os dados são divididos em conjuntos de treino e teste.
Um pipeline com StandardScaler e SVC (Support Vector Classification) é treinado para classificar os dados.
O modelo é avaliado quanto à acurácia, e são calculadas e exibidas métricas adicionais como a matriz de confusão, relatórios de classificação, e a curva ROC (Receiver Operating Characteristic).
Visualização e Métricas:

A curva ROC é plotada para avaliar a performance do modelo.
O código calcula e exibe a correlação das variáveis com a variável alvo (pep).
Este projeto demonstra um fluxo completo de preparação, análise e modelagem de dados para prever e entender padrões no conjunto de dados bancários, com visualizações e métricas para avaliar a eficácia dos modelos desenvolvidos.
