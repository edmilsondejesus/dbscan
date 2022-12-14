# *DBScan* - *Implementação do Algoritmo de Agrupamento baseado em Densidade*


## Descrição
- Algoritmo de agrupamento baseado em densidade, formando uma partição com formato arbitrário, podendo não ser um formato esférico.  Uma das pricipais vantágens é que  não é necessário informar o K ( número de grupos). No entanto, torna-se obrigatório informar outros hiperparâmetros, como o raio e o número mínimo de pontos.

- DBSCAN é uma abreviação do termo ‘Density Based Spatial Clustering of Application with Noise’ (Clusterização Espacial Baseada em Densidade de Aplicações com Ruído) é um método de clusterização não paramétrico baseado em densidade, proposto por ESTER et al (1996).

## Vantagens
- Identifica os ruídos e não confunde com grupos
- Não é necessário informar o número de grupos (K)

## Desvantagens
- Necessário informar dois parâmetros, o raio máximo de vizinhança e o número mínimo de pontos. 

## Aplicação
- Aplicável a qualquer base de dados contendo dados de um espaço métrico

## Implementação
Dados de entrada:
- a) Raio: raio máximo da vizinhança (também conhecido como epsilon);
- b) minPoints: número mínimo de pontos em um raio de vizinhança para um dado ponto;
- c) funcao_distancia: método de cálculo da medida de distância entre os pontos no espaço;
- d) X: Dataset do conjunto de dados.

 
1. Calcula a matriz de distâncias entre todos os pontos;
2. Identifica os pontos de vizinhança relativos a cada ponto, observando o critério de raio máximo;
3. Varre todos os pontos para encontrar os ruídos, os corepoints e os agrupamentos conectados recursivamente;
4. Por fim, exibe o gráfico de visualização dos pontos do dataset, antes e após a predição de agrupamento;
5. Na seção "Testando a Classe DBScan" são mostradas dois exemplos de aplicação do agrupamento por DBScan.

## Base de dados
- UCI - IRIS Dataset: https://archive.ics.uci.edu/ml/datasets/iris


## Referências
- https://www.maxwell.vrac.puc-rio.br/24787/24787_6.PDF
- https://medium.com/analytics-vidhya/dbscan-from-scratch-almost-b02096600c14
- https://www.youtube.com/watch?v=ETmqmmhMOR8&t=476s
- https://www.youtube.com/watch?v=RDZUdRSDOok
- https://github.com/abmorte/dbscan
- Atividade da Disciplina MATE33 Aprendizado Não Supervisonado do PGCOMP-UFBA 2022/02