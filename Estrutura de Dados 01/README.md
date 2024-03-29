# Faculdade Diagrama  de Dijkstran

 **_Algoritmo Dijkstra é um algoritmo para encontrar os caminhos mais curtos entre os nós de um gráfico_**

O porto de Santos é o vértice indicado pelo número 5 (cinco). As demais regiões são representadas pelos demais vértices que vão de 1 (um) a 4 (quatro). 

Você foi convidado a desenvolver uma solução que ajude a empresa em uma tomada de decisão, pois devido ao aumento consecutivo do valor do diesel, a empresa quer uma estimativa de quais os menores custos para continuar operando no porto de Santos. Foi feito um levantamento histórico com o custo médio de operação em cada ponto de origem até o destino final.  

No contexto da figura, os vértices 1, 2, 3, 4 e 5 representam, respectivamente as regiões cidades em que a transportadora opera hoje. O trajeto é representado pelas arestas que liga (1 a 2), (1 a 3), (2 a 4), (2 a 5), e assim por diante. O custo médio (peso) entre cada conexão está representado por X. Você deve substituir o X pelos 7 primeiros dígitos do seu RA (indo da esquerda para direita) multiplicado por 100, na sequência: (1-2), (1-3), (2-4), (2-5), (3-2), (3-5), (4-5).  

Exemplo:  

RA 2025703-5 = Será utilizado os seguintes números do seu RA 2025703  

RA 202570-5 = Em caso de 6 dígitos, acrescentar o dígito 1 ao final 2025701  

(1-2) = 2 * 100 = 200
(1-3) = 0 * 100 = 0
(2-4) = 2 * 100 = 200
......

Considerando que você precisa desenvolver a solução, utilize o algoritmo de Dijkstra e informe o caminho de menor custo saindo de 1 (que é a matriz da empresa em Mato Grosso do Sul) e chegando em 5. O resultado do seu programa deverá indicar as rotas que poderão ser utilizadas pela companhia e o seu respectivo peso.  

Passos para realizar o Mapa:  

1. Desenvolva um programa em linguagem C, salvar com a extensão (.c) que informe os caminhos saindo de 1 e chegando em 5.  

1.1. Neste código, usuário deverá excetuar as seguintes ações:
   - informar o número de vértices (ponto de rota),
   - informar as arestas com suas respectivas rotas de origem e destino,
   - informar o custo correspondente ao seu RA para todas as rotas.

1.2. Cálcular rotas.  

1.3. Apresentar na tela todos os destinos com os seus respectivos pesos. 

