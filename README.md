# Project Comportamento do Consumidor
  Status(Active)
# Project objective
  Utilizando o Dataset de comportamento do consumidor o objetivo é utilizar algoritimos não supervisionados de clusterização, para tornar as ações de marketing
  da empresa mais efetivas, diminuindo o custo de suas operações. Além disso, através de um modelo surpevisionado de regressão, o cadastro de novos clientes irá
  prever quanto esse cliente ira gastar ao longo dos proximos anos com a determinada loja. A junção desses dois modelos irá direcionar a empresa para a aquisição 
  de melhores clientes, otimizando sua receita e diminuindo seu CAC.
  
# Methods
  List with methods:
   - Limpeza de Dados
   - Tratamento de colunas
   - EDA
   - Clusterização (KMenas e Mistura Gaussiana)
   - Regressão (GDB)
# Technologies 
  - Python
  - Pandas
  - Seaborn
  - Matplotlib
  - Sklearn
  - Pycaret
  - Yellowbricks
# Project Description
  O Dataset possui 2240 linhas e 29 colunas, tais colunas podem ser categorizadas em três grupos - Informações do Consumidor, Gasto por produto, Lugar
  da compra e as promoções. Após a análise exploratória das variáveis, remoção de outliers e tratamento das colunas, transformando todas em numéricas, utilizei
  modelos não supervisionados de clustering, para identificar os principais grupos e quais grupos são mais propensos a aceitarem as promoções, tornando assim o 
  as ações da empresa sobre o cliente mais efetivas. Além disso, utilizando as informações de gasto por produto e os clusters antes criado, elaborei um modelo de 
  regressão supervisionado, o qual busca prever quais são as principais características que refletem no consumo e assim otimizar o CAC da empresa.
 

# Steps
  1. Leitura do Dataset e identificar a quantidade de nulos (0,5%).
  2. Eliminação dos nulos, Dataset fica com 2216 linhas
  3. Tratamento de colunas categóricas (Educação, Status de Relacionamento, Filhos e Tamanho da Família )
  3. Tratamento de colunas numéricas (Idade, Quantidade de dinheiro gasto e Tempo de relacionamento com a loja)
  4. Análise Exploratória para identificar outliers e entender o comportamento dos dados.
  5. Através da visualização foram identificados outliers, os quais foram removidos do Dataset.
  6. Como o Dataset contem muitas colunas (29), criei dois DataFrames para rodar os modelos. O primeiro continha todas as colunas e o segundo apenas as colunas demográficas.
  7. O primeiro algorítmo de clusterização foi o PCA. Esse reduz a dimensionalidade do Dataframe, facilitando na visualização e no entendimento dos componentes.
  8. Depois do PCA, utilizei o KMeans, com os dois grupos criados anteriormente e utilizei o resultado do PCA para rodar um terceiro KMeans.
  9. Por fim, utilizei Mistura Gaussiana como terceiro algoritmo não surpevisionado de clusterização.
  10. Vale lembrar, que os modelos utilizam distancia, assim os dados foram normalizados e as métricas de avaliação foram o método do cotovelo e silhueta.
  11. O modelo que melhor performou foi o KMeans com o grupo feito pelo PCA. Dessa maneira foi elaborado 5 grupos.
  12. Depois da formação de clusters utilizei a biblioteca Pycaret para otimizar o modelo de classificação. O modelo utilizado foi Gradient Boosting Classifier.
  13. A métrica otimizada foi a Recall, uma vez que faz sentido para o negócio identificar quem aceitaria a propaganda.
  14. Ainda utilizando o Pycaret, o modelo de regressão utilizado foi a Random Forest e a métrica foi o R2
  15. O resultado do GBC foi de 88.75% e o R2 da regressão foi de 85%.

# Conclusion
  Os homens são sem duvidas mais atacados por tubarões em quase todas as regiões do mundo, as principais atividades que originam ataques, são surfe, nadar no mar e pesca,
  sobre essas atividades é interessante ver como a atividade de pesca é em grande parte praticada por homens, uma vez que existe uma grande diferença nos ataques feito as mulheres pescando. 
 Além disso é interessante ver como os ataques as mulheres vêm aumentando nos últimos anos, uma vez que o número de ataques estão se equalizando independente do gênero.
 Hoje as atividades/esportes não apresentam mais barreiras em relação a sexo, assim é comum ver mulheres se aventurando mais e praticando atividades/esportes que antes eram centralizadas e comercializadas sobre o sexo masculino.
  
# Contact
  Linkedin: https://www.linkedin.com/in/lucas-perfeito-0a55381ab/ 
  
