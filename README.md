# Classificação do Conjunto de Dados Íris

Este projeto utiliza técnicas de aprendizado de máquina para classificar as diferentes espécies de flores do conjunto de dados Íris. Foram implementados três modelos de classificação: K-Nearest Neighbors (KNN), Árvore de Decisão e Support Vector Machine (SVM) com kernel RBF.

## Conjunto de Dados

## Conjunto de Dados Íris

O conjunto de dados Íris é um dos conjuntos de dados mais famosos e amplamente utilizados em aprendizado de máquina. Ele foi introduzido pela primeira vez pelo estatístico e biólogo britânico Ronald Fisher em seu artigo de 1936 intitulado "The Use of Multiple Measurements in Taxonomic Problems" (*O Uso de Múltiplas Medidas em Problemas Taxonômicos*).

<center><img alt="Analisando Airbnb" width="100%" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cb/Flores_de_%C3%8Dris.png/1920px-Flores_de_%C3%8Dris.png"></center>




Este conjunto de dados é composto por medidas de comprimento e largura das sépalas e pétalas de três espécies diferentes de flores Íris: setosa, versicolor e virginica. Cada espécie é representada por 50 amostras, totalizando 150 amostras no conjunto de dados. As medidas foram obtidas de 50 flores de cada espécie, coletadas na Ilha de Gough e na Península do Monte Oread, ambas na América do Sul.

As quatro características do conjunto de dados Íris são:

1. Comprimento da Sépala (em centímetros)
2. Largura da Sépala (em centímetros)
3. Comprimento da Pétala (em centímetros)
4. Largura da Pétala (em centímetros)

## Modelos Implementados

### K-Nearest Neighbors (KNN)

#### Teoria:

O K-Nearest Neighbors (KNN) é um algoritmo de aprendizado supervisionado utilizado para problemas de classificação e regressão. Ele classifica um ponto de dado com base na maioria dos seus vizinhos mais próximos no espaço de características. A distância entre os pontos é geralmente medida usando a distância Euclidiana.

#### Representação Matemática:

A previsão do KNN é baseada na votação da classe dos $ k $ vizinhos mais próximos de um ponto de dado de teste. A previsão é dada por:


$$ hat{y} = \text{mode}(y_{i_1}, y_{i_2}, ..., y_{i_k}) $$


onde $y_{i_1}, y_{i_2}, ..., y_{i_k}$ são as classes dos $k$ vizinhos mais próximos e $\text{mode}$ retorna a classe mais frequente.

### Árvore de Decisão


A Árvore de Decisão é um modelo baseado em regras que divide o espaço de características em regiões homogêneas por meio de uma série de perguntas. O objetivo é criar uma árvore de decisão que melhor divide os dados em classes distintas.

#### Representação Matemática:

A Árvore de Decisão pode ser representada matematicamente por uma sequência de regras de decisão. Cada nó interno da árvore representa uma condição de divisão em um atributo, e os ramos representam os resultados dos testes. Os nós folhas representam as classes ou valores de saída.

### Support Vector Machine (SVM) com kernel RBF


O Support Vector Machine (SVM) é um modelo de aprendizado supervisionado utilizado para classificação e regressão. Com o uso do kernel RBF, o SVM mapeia os dados para um espaço de características de alta dimensão e encontra uma fronteira de decisão não linear.

#### Representação Matemática:

A formulação do SVM com kernel RBF pode ser expressa como a minimização de uma função objetivo sujeita a restrições. A função objetivo é dada por:


$$\min_{\mathbf{w}, b, \xi} \quad \frac{1}{2} \|\mathbf{w}\|^2 + C \sum_{i=1}^{n} \xi_i$$


onde  $\mathbf{w}$ é o vetor de pesos, $b$ é o termo de polarização, $\xi$ são as variáveis de folga e $C$ é o parâmetro de regularização.

## Resultados

Os resultados dos modelos no conjunto de dados de teste são os seguintes:

## Resultados dos Modelos

### KNN:

|               | Precision | Recall | F1-Score | Support |
|---------------|-----------|--------|----------|---------|
| Iris-setosa   |    1.00   |  1.00  |   1.00   |    15   |
| Iris-versicolor |   1.00   |  1.00  |   1.00   |    9    |
| Iris-virginica |    1.00   |  1.00  |   1.00   |    6    |
|    Accuracy   |           |        |   1.00   |    30   |
|   Macro Avg   |   1.00    |  1.00  |   1.00   |    30   |
| Weighted Avg  |   1.00    |  1.00  |   1.00   |    30   |

### Árvore de Decisão:

|               | Precision | Recall | F1-Score | Support |
|---------------|-----------|--------|----------|---------|
| Iris-setosa   |    1.00   |  1.00  |   1.00   |    15   |
| Iris-versicolor |   0.89   |  0.89  |   0.89   |    9    |
| Iris-virginica |    0.83   |  0.83  |   0.83   |    6    |
|    Accuracy   |           |        |   0.93   |    30   |
|   Macro Avg   |   0.91    |  0.91  |   0.91   |    30   |
| Weighted Avg  |   0.93    |  0.93  |   0.93   |    30   |

### SVM com kernel RBF:

|               | Precision | Recall | F1-Score | Support |
|---------------|-----------|--------|----------|---------|
| Iris-setosa   |    1.00   |  1.00  |   1.00   |    15   |
| Iris-versicolor |   1.00   |  0.89  |   0.94   |    9    |
| Iris-virginica |    0.86   |  1.00  |   0.92   |    6    |
|    Accuracy   |           |        |   0.97   |    30   |
|   Macro Avg   |   0.95    |  0.96  |   0.95   |    30   |
| Weighted Avg  |   0.97    |  0.97  |   0.97   |    30   |


## Conclusão

O KNN, a Árvore de Decisão e o SVM com kernel RBF são modelos eficazes para a classificação do conjunto de dados Íris. Cada modelo tem suas próprias vantagens e limitações, e a escolha do modelo mais adequado depende da natureza dos dados e dos requisitos do problema.

## Outros projetos e Portifólio:
Outros projetos de minha autoria e meu portifólio:

* **Analise de dados do Airbnb Los Angeles:** https://github.com/JpLimags/Analise_dados_Airbnb
* **Como Implementar Regressão Linear com Python:** https://github.com/JpLimags/Portifolio
