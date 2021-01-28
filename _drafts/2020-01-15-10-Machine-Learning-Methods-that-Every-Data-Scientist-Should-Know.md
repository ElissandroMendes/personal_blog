---
layout: post
title:  "10 Métodos de Aprendizado de Máquina que todo Cientista de dados deveria conhecer"
date:   2020-01-15 22:53:00 +0300
image:  foto-post-ml.jpg
tags:   Aprendizado-de-Máquina Ciência-de-Dados
---
Aprendizado de máquina é um tema quente seja na academia ou na indústria, com novas metodologias sendo desenvolvidas o tempo todo. A velocidade e complexidade das novas técnicas que são desenvolvidas traz dificuldades mesmo para experts - e potencialmente sobrecarregará os iniciantes.

Para desmistificar a aprendizagem de máquina e oferecer um caminho para aqueles que ainda não conhecem bem os conceitos principais, vamos dar uma olhada em 10 diferentes métodos, incluindo uma descrição, visualizações e exemplos para cada um.

Um algoritmo de aprendizado de máquina, também chamado de modelo, é uma expressão matemática que representa a informação num contexto de um problema, quase sempre um problema de negócio. O objetivo é, partindo da informação, gerar insight. Por exemplo, se um comerciante que antecipar as vendas para o próximo quadrimestre, ele pode usar um algoritmo que preveja as vendas com base na vendas passadas e outras informações relevantes. De forma semelhante, um 
fabricante de moinho de vento pode monitorar visualmente um equipamente importante, alimentando algoritmos com as imagens, treinando-os assim para prever possíveis rachaduras perigosas.

Os 10 métodos aqui descritos oferecem uma visão geral - e voce poderá aprofundar a medida que desenvolve seus conhecimentos de aprendizagem de máquina.

1. *Regressão*
2. *Classificação*
3. *Clusterização*
4. *Redução de dimensionalidade*
5. *Ensemble de métodos*
6. *Redes neurais e Aprendizado profundo*
7. *Aprendizado por transferência*
8. *Aprendizado por reforço*
9. *Processamento de linguagem natural*
10. *Word Embeddings* 


Uma última coisa antes de iniciarmos. Vamos distinguir entre duas categorias de gerais de aprendizagem de máquina: supervisionado e não supervisionado. Aplicamos técnicas de ML supervisionado quando temos partes da informação que queremos predizer ou explicar. Fazemos isso usando dados de entrada e saída previamente conhecidos para predizer a resposta para novos dados de entrada. Por exemplo, podemos usar técnicas supervisionadas para ajudar um serviço a predizer quantos uduário irão se inscrever nele no mês que vem. Já no aprendizado não supervisionado buscamos maneira de relacionar e agrupar dados sem o uso de uma variável alvo a ser predita. Em outras palavras, os dados serão avaliados com base em suas características e com base nelas forma-se clusters de itens que são similares entre si. Por exemplo, podemos ajudar um comerciante a agrupar produtos similares sem necessariamente nos preocupar em selecionar que características usar.
---
## Regressão
Métodos de regresão fazem parte de uma categoria de ML chamada de *supervisionada*. Eles ajudam a predizer ou explicar um valor númerico em particular baseado num conjunto de dados conhecidos, por exemplo, predizer o preço de uma propriedade baseado-se nos preços de propriedades semelhantes.

O método mais simples de regressão linear é aquela em que usamos a seguinte equação, y = m * x + b, para modelar nossos dados. Treinamos um modelo de regressão linear com pares de dados (x, y) calculando a posção e a inclinação de uma reta que minimiza a distância total entre todos os pontos de dados e a reta. 

Em outras palavra, calculamos a inclinação (m) e o valor que interceptamos o eixo y (b) para uma linha que melhor aproxime as observações em nossos dados.


The simplest method is linear regression where we use the mathematical equation of the line (y = m * x + b) to model a data set. We train a linear regression model with many data pairs (x, y) by calculating the position and slope of a line that minimizes the total distance between all of the data points and the line. In other words, we calculate the slope (m) and the y-intercept (b) for a line that best approximates the observations in the data.

Let’s consider a more a concrete example of linear regression. I once used a linear regression to predict the energy consumption (in kWh) of certain buildings by gathering together the age of the building, number of stories, square feet and the number of plugged wall equipment. Since there were more than one input (age, square feet, etc…), I used a multi-variable linear regression. The principle was the same as a simple one-to-one linear regression, but in this case the “line” I created occurred in multi-dimensional space based on the number of variables.

The plot below shows how well the linear regression model fit the actual energy consumption of building. Now imagine that you have access to the characteristics of a building (age, square feet, etc…) but you don’t know the energy consumption. In this case, we can use the fitted line to approximate the energy consumption of the particular building.

Note that you can also use linear regression to estimate the weight of each factor that contributes to the final prediction of consumed energy. For example, once you have a formula, you can determine whether age, size, or height is most important.
