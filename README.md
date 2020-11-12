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
|[2-FullIns_3](instances/VC/2-FullIns_4.col)      |52   |201  |4   |
|[2-FullIns_4](instances/VC/2-FullIns_4.col)      |212   |1621  |6   |
|[4-FullIns_3](instances/VC/4-FullIns_3.col)      |114   |541  |7   |
|[5-FullIns_3](instances/VC/5-FullIns_3.col)      |154   | 792  |3   |
|[queen5_5](instances/VC/queen5_5.col)    |25  |160  |5  |
|[queen6_6](instances/VC/queen6_6.col)    |36  |290  |6  |
|[queen7_7](instances/VC/queen7_7.col)    |49  |476	  |7  |
|[queen9_9](instances/VC/queen9_9.col)  |81  |1056  |9  |
|[queen10_10](instances/VC/queen10_10.col)      |100   |2940  |11   |
|[queen11_11](instances/VC/queen11_11.col)    |121  |3960  |11   |


__Note 1:__ As instâncias e os melhores resultados conhecidos foram retirados de [site da instâncias](https://sites.google.com/site/graphcoloring/vertex-coloring).

__Note 2:__ Um modelo de programação linear e detalhes do problema, podem ser encontrada em [Malaguti et al. (2011)](https://www.sciencedirect.com/science/article/pii/S157252861000054X).


### The Minimum Labeling Spanning Trees

As instâncias com nome "testFile" foram produzidas para esta cadeira, e foram testadas usando o solver GLPK, durante duas horas no modelo definido em  [descricao_problemas.pdf](descricao_problemas.pdf), valores com * do lado representam solução otima encontradas dentro de duas horas pelo solver. As instâncias sem o nome testFile são instâncias usadas no trabalho [Cerulli et al. (2014)](https://www.sciencedirect.com/science/article/pii/S1877042813054682#:~:text=In%20the%20k%2Dlabeled%20Spanning,most%20kmax%20different%20labels.)

Essas instâncias são definidas por uma linha definindo o número de vértices, arestas e rótulos respectivamente, seguida por uma linha em branco e |E| linhas que definem no formato (v1 v2 l) as arestas com extremos v1 e v2 e rótulo l.

| Instance | \|_N_\| | \|_E_\| |  \|_L_\| |  BKS|
|----------|-------:|---------:|------:|------:|
|[testFile_0_10_5 ](instances/MLST/testFile_0_10_5.col) | 10 | 9 | 5 | 5* |
|[testFile_7_75_37](instances/MLST/testFile_7_75_37.col) | 75  | 555 | 37 | 10 |
|[testFile_9_75_60](instances/MLST/testFile_9_75_60.col) | 75  | 555 | 60| 7* |
|[testFile_11_75_93](instances/MLST/testFile_11_75_93.col) | 75  | 555 |  93 | 20 |
|[100-990-25-3-1](instances/MLST/100-990-25-3-1) | 100  | 990 | 25 | 8 |
|[100-990-25-3-4](instances/MLST/100-990-25-3-4) | 100  | 990 | 25 | 5 |
|[100-990-50-6-7](instances/MLST/100-990-50-6-7) | 100 | 990 | 50 | 14 |
|[100-990-50-6-8](instances/MLST/100-990-50-6-8) | 100 | 990 | 50  | 7 |
|[100-990-100-6-5](instances/MLST/100-990-100-6-5) | 109 | 990 | 100 | 17 |
|[100-990-125-7-4](instances/MLST/100-990-125-7-4) | 100 | 990 | 125 | 11  |

__Note 1:__ Um modelo de programação linear e detalhes do problema, podem ser encontrada em [Captivo et al. (2009)](https://www.sciencedirect.com/science/article/abs/pii/S0305054809000458).

### The k-labeled Spannig Forest

As instâncias com nome "testFile" foram produzidas para esta cadeira, e foram testadas usando o solver GLPK, durante duas horas no modelo definido em  [descricao_problemas.pdf](descricao_problemas.pdf), valores com * do lado representam solução otima encontradas dentro de duas horas pelo solver. As instâncias sem o nome testFile são instâncias usadas no trabalho [Cerulli et al. (2014)](https://www.sciencedirect.com/science/article/pii/S1877042813054682#:~:text=In%20the%20k%2Dlabeled%20Spanning,most%20kmax%20different%20labels.), e os best know delas foram delas foram retirado de. [Figueredo (2020]

Essas instâncias são definidas por uma linha definindo o número de vértices, arestas, rótulos e o valor k_max respectivamente, seguida por uma linha em branco e |E| linhas que definem no formato (v1 v2 l) as arestas com extremos v1 e v2 e rótulo l.


| Instance | \|_N_\| | \|_E_\| |  \|_L_\||  k_max|  BKS|
|:---------|----------:|-----:|------:|------:|------:|
|[testFile_0_10_5 ](instances/kLSF/testFile_0_10_5.col) | 10 | 9  | 5  | 3 | 4* |
|[testFile_7_75_35  ](instances/kLSF/testFile_1_50_25.col) | 75 | 555 | 35 | 4 | 17 |
|[testFile_9_75_60](instances/kLSF/testFile_4_50_40.col) | 75 | 555 | 60 | 5 | 7* |
|[testFile_11_75_93](instances/kLSF/testFile_6_50_62.col) | 75 | 555 | 93 | 6 | 11* |
|[100-990-25-3-1](instances/kLSF/100-990-25-3-1) | 100  | 990 | 25 | 3 | 7* |
|[100-990-25-3-4](instances/kLSF/100-990-25-3-4) | 100  | 990 | 25 | 3 | 7* |
|[100-990-50-6-7](instances/kLSF/100-990-50-6-7) | 100 | 990 | 50 | 6 | 1* |
|[100-990-50-6-8](instances/kLSF/100-990-50-6-8) | 100 | 990 | 50  | 6 | 3* |
|[100-990-100-6-5](instances/kLSF/100-990-100-6-5) | 109 | 990 | 100 | 6 | 20* |
|[100-990-125-7-4](instances/kLSF/100-990-125-7-4) | 100 | 990 | 125 | 7  | 16* |


__Note 1:__ Um modelo de programação linear e detalhes do problema, podem ser encontrada em [Figueredo (2020)](http://www.repositorio.ufc.br/bitstream/riufc/50722/3/2020_dis_pjafigueredo.pdf).

### Duvidas

Duvidas podem me contatar pelo email tiago.drehmer@gmail.com

### Atualizações

Atualização (31/10/2020)
- Instâncias foram padronizadas.
- Best Know atualizado de algumas que não tinham.
- Corrigido links quebrado

Atualização (31/10/2020)
- Instâncias do vertice covering foram alteradas
  - Alterei algumas instância pois foi o problema com maior exigência em relação ao tamanho delas, então reduzi algumas.
  
Atualização (12/11/2020)
  - Corrigido algumas arestas que tava duplicada nos arquivos do MST e kLSF
  - Corrigido a otimilidade do kLSF

