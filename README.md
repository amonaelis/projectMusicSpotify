# Insight sobre o Projeto
Objetivo do Projeto:
Classificar músicas como "Música agitada" ou "Música lenta" com base na coluna "valence".

Estrutura do Projeto
Leitura e Pré-processamento dos Dados:
Os dados foram lidos de um arquivo Excel (novos_dados.xlsx).
As variáveis categóricas, como track_genre, foram codificadas utilizando LabelEncoder.
Os dados foram normalizados para garantir que todas as features estivessem na mesma escala.

Treinamento do Modelo:
Um modelo de Random Forest foi treinado e ajustado utilizando GridSearch para otimização dos hiperparâmetros.
Após o treinamento, o modelo foi usado para prever a classificação das músicas.

Classificação e Mapeamento:
As previsões feitas pelo modelo foram mapeadas para rótulos compreensíveis: "Música agitada" para o valor 0 e "Música lenta" para o valor 1.
Os resultados foram então adicionados de volta à base de dados original em uma nova coluna target.
