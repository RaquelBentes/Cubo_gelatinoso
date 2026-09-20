# Cubo Gelatinoso: Classificação de tipo espectral de estrelas com k-NN
Projeto de Aprendizado de máquina introdutório do uso de K-NN.

## Descrição do Projeto

Este projeto foi desenvolvido para a disciplina de "Aprendizado de máquina" do curso interdisciplinar de Bacharelado em Ciência e Tecnologia da Ilum Escola de ciência. Sua aplicação envolve o uso do algoritmo k-vizinhos mais próximos (k-NN) para classificar o tipo espectral principal de estrelas (O, B, A, F, G, K, M,  além das raras C, S e W), a partir de uma amostra de 2000 estrelas mais brilhantes do catálogo HYG Database. Os atributos utilizados foram magnitude aparente, magnitude absoluta, distância, color index e hemisfério em que essa estrela se encontra.

## Estrutura do repositório

- `cubo_gelatinoso.ipynb`: notebook principal com todo o desenvolvimento (coleta e tratamento de dados, análise exploratória, normalização, codificação de atributos, treino/teste, baseline e modelo k-NN);
- `hyg_v44.csv.gz`: conjunto de dados utilizado (catálogo HYG).

## Instalação e Instruções

Requer Python 3 com as bibliotecas: pandas, numpy, scikit-learn, seaborn, matplotlib. Basta abrir o notebook em um ambiente Jupyter e executar as células em ordem, de cima para baixo.

## Principais resultados

O modelo k-NN (n_neighbors=3, p=2) atingiu 67% de acurácia balanceada, frente a 14% do modelo baseline (DummyClassifier). Também foi observado que a normalização dos dados teve grande impacto no desempenho (67% com normalização vs. 38% sem ela), enquanto a estratégia de codificação do atributo categórico (OneHotEncoder vs. OrdinalEncoder) não gerou diferença significativa.

## Professor orientador:
### Daniel Roberto Cassar
Doutor em Ciência e Engenharia de Materiais pela Universidade Federal de São Carlos (UFSCar, 2014). Atualmente é Professor Assistente no Bacharelado em Ciência e Tecnologia da Ilum Escola de Ciência, parte do Centro Nacional de Pesquisa em Energia e Materiais (CNPEM)

## Autoria
### Raquel Bentes Lima
Estudante de bacharelado em Ciência e Tecnologia na Ilum Escola de Ciência.
