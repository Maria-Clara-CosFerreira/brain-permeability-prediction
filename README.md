<img width="2480" height="254" alt="Cabecalho" src="https://github.com/user-attachments/assets/88a9125e-ce2e-428f-b913-f082ade21d68" />

# Predição da Permeabilidade pela Barreira Hematoencefálica

## Projeto da Disciplina de Aprendizado de Máquina

Instituição de ensino vinculada à desenvolvedora do projeto: Ilum Escola de Ciência - CNPEM (Centro Nacional de Pesquisa em Energia e Materiais)

## Autora

Maria Clara Costa Ferreira

## Descrição do projeto

Este projeto consiste na aplicação de algoritmos de aprendizado de máquina para a classificação de moléculas quanto à sua capacidade de atravessar a barreira hematoencefálica (Blood-Brain Barrier — BBB), utilizando descritores moleculares para representar suas características químicas e estruturais.

O objetivo é desenvolver modelos capazes de prever se uma molécula apresenta permeabilidade à barreira hematoencefálica (BBB+) ou não (BBB−), a partir de suas propriedades moleculares. Para isso, são utilizados dados do dataset B3DB, que reúne informações sobre moléculas e suas respectivas classificações de permeabilidade.

Foram desenvolvidos e comparados diferentes modelos de classificação, utilizando os algoritmos Logistic Regression, K-Nearest Neighbors (KNN) e Random Forest. Também foi utilizado o Dummy Classifier como modelo de referência (baseline).

O pré-processamento dos dados inclui o tratamento de valores ausentes, a remoção de atributos sem variabilidade e a seleção de características relevantes. Para otimizar os hiperparâmetros dos modelos, foi utilizada a biblioteca Optuna, em conjunto com validação cruzada.

A avaliação dos modelos é realizada por meio de métricas de classificação, permitindo comparar seu desempenho e investigar sua capacidade de generalização para moléculas não utilizadas durante o treinamento.

## Organização do repositório

### Notebook principal

* Trabalho-Final.ipynb

O notebook contém a implementação do projeto, incluindo:

* Introdução teórica sobre a barreira hematoencefálica e a predição de sua permeabilidade;
* Carregamento e exploração dos dados do Tiamat;
* Análise da distribuição das classes;
* Análise de valores ausentes e duplicatas;
* Preparação dos descritores moleculares;
* Separação dos dados em conjuntos de treino e teste;
* Construção de pipelines de pré-processamento e classificação;
* Implementação dos modelos de Regressão Logística, KNN, Random Forest e HistGradientBoosting;
* Utilização do Dummy Classifier como baseline;
* Otimização de hiperparâmetros utilizando Optuna;
* Validação cruzada;
* Avaliação dos modelos por meio de métricas de classificação;
* Análise e comparação dos resultados.

## Dataset

Foi utilizado o dataset Tiamat, contendo informações moleculares e classificações relacionadas à permeabilidade da barreira hematoencefálica.

As moléculas são representadas por estruturas químicas, expressas por meio de SMILES, e por descritores moleculares numéricos que representam diferentes propriedades químicas e estruturais.

O atributo utilizado como alvo da classificação é BBB+/BBB−, que indica se a molécula é capaz de atravessar a barreira hematoencefálica (BBB+) ou não (BBB−).

## Como executar

1. Abra o notebook principal do projeto.
2. Certifique-se de que o dataset utilizado esteja disponível no ambiente de execução.
3. Instale as bibliotecas necessárias.
4. Execute as células do notebook na ordem em que aparecem.
5. Acompanhe as etapas de exploração dos dados, pré-processamento, otimização e treinamento dos modelos.
6. Ao final, observe as métricas e visualizações utilizadas para comparar o desempenho dos classificadores.

## Bibliotecas utilizadas

* pandas — organização, manipulação e análise dos dados;
* NumPy — operações numéricas e manipulação de arrays;
* scikit-learn — pré-processamento, seleção de características, construção de pipelines, treinamento dos modelos, validação cruzada e avaliação dos classificadores;
* Optuna — otimização de hiperparâmetros dos modelos;
* RDKit — processamento de estruturas químicas e manipulação de moléculas representadas por SMILES;
* seaborn — criação de visualizações estatísticas;
* matplotlib — criação e personalização de gráficos;
* warnings — controle da exibição de avisos durante a execução do código.
