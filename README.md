# INF05010 - Otimização Combinatoria

Esse repositorio contem uma apresentação dos problemas para o trabalho em [descricao_problemas.pdf](descricao_problemas.pdf). E uma explicação mais detalhada do projeto em  [especificacoes_projeto.pdf](especificacoes_projeto.pdf).

## Instancias dos problemas

Nas seguintes tabelas são apresentadas o numeros de vertices |V| o numero de arestas |E| e os melhores valores conhecido MRC.
### Vertex Coloring

As instâncias a seguir são definidas por

c - linha de comentarios

e n1 n2 - aresta definida pelos extremos n1 e n2

| Instance | \|_V_\| | \|_E_\| | MRC|
|----------|-------:|---------:|------:|
|[2-FullIns_4](instances/CG/2-FullIns_4.col)      |212   |1621  |6   |
|[4-FullIns_3](instances/CG/4-FullIns_3.col)      |114   |541  |7   |
|[5-FullIns_3](instances/CG/5-FullIns_3.col)      |154   | 792  |3   |
|[queen10_10](instances/CG/queen10_10.col)      |100   |2940  |11   |
|[queen11_11](instances/CG/queen11_11.col)    |121  |3960  |11   |
|[queen12_12](instances/CG/queen12_12.col)    |244  |5192  |12  |
|[queen13_13](instances/CG/queen13_13.col)    |169  |6656  |13  |
|[queen14_14](instances/CG/queen14_14.col)    |196  |4186	  |14  |
|[queen15_15](instances/CG/queen15_15.col)  |225  |5180  |15  |
|[queen16_16](instances/CG/queen16_16.col)  |256  |12640  |17  |


__Note 1:__ As instâncias e os melhores resultados conhecidos foram retirados de [site da instâncias](https://sites.google.com/site/graphcoloring/vertex-coloring).

__Note 2:__ Um modelo de programação linear e detalhes do problema, podem ser encontrada em [Malaguti et al. (2011)](https://www.sciencedirect.com/science/article/pii/S157252861000054X).


### The Minimum Labeling Spanning Trees

As instancias com nome "testFile" foram produzidas para esta cadeira, e foram testadas usando o solver GLPK, durante duas horas no modelo definido em  [descricao_problemas.pdf](descricao_problemas.pdf), valores com * do lado representam solução otima encontradas dentro de duas horas pelo solver. As instancias com nome cerulli são instancias usadas no trabalho [Cerulli et al. (2014)](https://www.sciencedirect.com/science/article/pii/S1877042813054682#:~:text=In%20the%20k%2Dlabeled%20Spanning,most%20kmax%20different%20labels.), e não possuem resultados ainda pois não rodei o solver nelas, assim que tiver resultados faço o update. 

Essas instancias são definidas por uma linha definindo o numero de vertices, arestas e rotulos respectivamente, seguida por |E| linhas que definem no formato (v1 v2 l) as arestas com extremos v1 e v2 e rotulo l.

| Instance | \|_N_\| | \|_E_\| |  \|_L_\| |  BKS|
|----------|-------:|---------:|------:|------:|
|[testFile_0_10_5 ](instances/MAGR/testFile_0_10_5.col) | 10 | 9 | 5 | 5* |
|[testFile_7_75_37  ](instances/MAGR/testFile_7_75_37.col) | 75  | 555 | 37 | 10 |
|[testFile_8_75_37  ](instances/MAGR/testFile_8_75_37.col) | 75  | 555 | 37 | 5* |
|[testFile_9_75_60  ](instances/MAGR/testFile_9_75_60.col) | 75  | 555 |  60 | 7* |
|[testFile_10_75_60  ](instances/MAGR/testFile_10_75_60.col) | 75  | 555 | 60 | 12 |
|[testFile_11_75_93 ](instances/MAGR/testFile_11_75_93.col) | 75  | 555 | 93 | 20  |
|[testFile_12_75_93 ](instances/MAGR/testFile_12_75_93.col) | 75 | 555 | 93 | 19 |
|[cerulli_100_25 ](instances/MAGR/cerulli_100_25.col) | 100 | 990 | 25  | - |
|[cerulli_100_50](instances/MAGR/cerulli_100_50.col) | 109 | 990 | 50 | - |
|[cerulli_100_100](instances/MAGR/cerulli_100_100.col) | 100 | 990 | 100 | - |

__Note 1:__ Um modelo de programação linear e detalhes do problema, podem ser encontrada em [Captivo et al. (2009)](https://www.sciencedirect.com/science/article/abs/pii/S0305054809000458).

### The k-labeled Spannig Forest

As instancias com nome "testFile" foram produzidas para esta cadeira, e foram testadas usando o solver GLPK, durante duas horas no modelo definido em  [descricao_problemas.pdf](descricao_problemas.pdf), valores com * do lado representam solução otima encontradas dentro de duas horas pelo solver. As instancias com nome cerulli são instancias usadas no trabalho [Cerulli et al. (2014)](https://www.sciencedirect.com/science/article/pii/S1877042813054682#:~:text=In%20the%20k%2Dlabeled%20Spanning,most%20kmax%20different%20labels.), e não possuem resultados ainda pois não rodei o solver nelas, assim que tiver resultados faço o update. 

Essas instancias são definidas por uma linha definindo o numero de vertices, arestas, rotulos e o valor k_max respectivamente, seguida por |E| linhas que definem no formato (v1 v2 l) as arestas com extremos v1 e v2 e rotulo l.


| Instance | \|_N_\| | \|_E_\| |  \|_L_\||  k_max|  BKS|
|:---------|----------:|-----:|------:|------:|------:|
|[testFile_0_10_5 ](instances/FGMkR/testFile_0_10_5.col) | 10 | 9  | 5  | 3 | 4* |
|[testFile_1_50_25  ](instances/FGMkR/testFile_1_50_25.col) | 50 | 245 | 25 | 4 | 4* |
|[testFile_4_50_40  ](instances/FGMkR/testFile_4_50_40.col) | 50 | 245 | 40 | 5 | 8 |
|[testFile_6_50_62  ](instances/FGMkR/testFile_6_50_62.col) | 50 | 245 | 62 | 6 | 13 |
|[testFile_7_75_37  ](instances/FGMkR/testFile_7_75_37.col) | 75 | 555 | 37 | 4 | 7 |
|[testFile_9_75_60 ](instances/FGMkR/testFile_9_75_60.col) | 75 | 555 | 60 | 5 | 16 |
|[testFile_11_75_93 ](instances/FGMkR/testFile_11_75_93.col) | 75 | 555 | 93 | 6 | 22 |
|[cerulli_100_25 ](instances/FGMkR/cerulli_100_25.col) | 100 | 990 | 25  | 3 | - |
|[cerulli_100_50](instances/FGMkR/cerulli_100_50.col) | 100 | 990 | 50 | 6 | - |
|[cerulli_100_100](instances/FGMkR/cerulli_100_100.col) | 100 | 990 | 100 | 6 | - |


__Note 1:__ Um modelo de programação linear e detalhes do problema, podem ser encontrada em [Figueredo (2020)](http://www.repositorio.ufc.br/bitstream/riufc/50722/3/2020_dis_pjafigueredo.pdf).



