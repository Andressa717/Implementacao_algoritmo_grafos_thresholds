# Implementacao_algoritmo_grafos_thresholds

Este algoritmo, desenvolvido por Jacobs, Trevisan e Tura (2013) pode ser utilizado para localizar os autovalores da matriz de adjacência de grafos thresholds. A implementação foi realizada na linguagem Python e é resultado do estudo realizado para o meu TCC, que compreendeu toda a parte matemática que está por trás do funcionamento do algoritmo. 

# Grafo threshold:
Um grafo threshold de ordem n pode ser definido por meio de uma sequência binária (b_1, b_2, ... , b_n), onde b_i = 0 representa a adição de um vértice isolado e b_i = 1 representa a adição de um vértice dominante (adiciona-se um vértice e conecta-se esse vértice a todos os vértices previamente adicionados).

A sequência que define um grafo threshold sempre inicia com o número zero. Essa sequência será formada por blocos alternados de zeros e uns, onde o primeiro bloco será de zeros. Para facilitar a entrada de dados, pode-se reescrever essa sequência binária da forma (0^{r_1}, 1^{r_2}, 0^{r_3}, 1^{r_4}, ..., 1^{r_k}), onde os índices r_i, indicam a quantidade de zeros/uns de cada bloco.

# Entrada de dados:
Lista a, das quantidades de zeros e uns de cada bloco (os índices r_i);
Um número real arbitrário x.

# Processamento:
O programa transforma a lista a na sequência binária b que define o grafo threshold. Após, define a variável n (quantidade de vértices do grafo e também a ordem da matriz de adjacência) como a soma dos elementos da lista a e, em seguida, cria a lista d com n elementos, todos iguais ao valor x inserido pelo usuário. Logo após, são realizados os cálculos do algoritmo e os valores da lista d vão sendo atualizados. O número x inserido pelo usuário é um chute para ver se tal número é autovalor ou não. A quantidade de autovalores
- maiores que x é a quantidade de elementos positivos na saída de dados;
- iguais a x é a quantidade de elementos iguais a zero na saída de dados;
- menores que x é a quantidade de elementos negativos na saída de dados.

# Saída de dados:
Lista d dos elementos da diagonal principal da matriz diagonal D congruente à matriz A + xI.

# Referências:
Artigo onde foi publicado o algoritmo:
JACOBS, D. P.; TREVISAN, V.; TURA, F. Eigenvalue location in threshold graphs. Linear Algebra and its Applications, Elsevier, v. 439, p. 2762 - 2773, 2013. 
