# INF05010 - Otimização Combinatoria

Esse repositorio contem uma apresentação dos problemas para o trabalho em [descricao_problemas.pdf](descricao_problemas.pdf). E uma explicação mais detalhada do projeeto em  [especificacoes_projeto.pdf](especificacoes_projeto.pdf).

## Instancias dos problemas

### Intancias pra problema de coloração de grafos

As instâncias a seguir são definidas por

c - linha de comentarios

e n1 n2 - aresta definida pelos extremos n1 e n2

| Instance | \|_N_\| | \|_M_\| | BKS|
|----------|-------:|---------:|------:|
|[2-FullIns_4](instances/CG/3-FullIns_4.col)      |20   |10  |1592   |
|[3-FullIns_4](instances/CG/3-FullIns_4.cool)      |20   |20  |2270   |
|[5-FullIns_3](instances/CG/3-FullIns_4.col)      |60   | 5  |3663   |
|[queen10_10](instances/CG/queen10_10.col)      |60   |10  |3423   |
|[queen11_11](instances/CG/queen11_11.col)    |100  |60  |9395   |
|[queen12_12](instances/CG/queen12_12.col)    |500  |40  |28548  |
|[queen13_13](instances/CG/queen13_13.col)    |500  |60  |31125  |
|[queen14_14](instances/CG/queen14_14.col)    |600  |20  |31433  |
|[queen15_15](instances/CG/queen15_15.col)  |700  |20  |36417  |
|[queen16_16](instances/CG/queen16_16.col)  |700  |20  |36417  |


__Note :__ As instancias foram tiradas e as melhores soluções foram tira das [site da instâncias](https://sites.google.com/site/graphcoloring/home).

__Note 2:__ A mathematical formulation of the problem can be found in [Tseng et al. (2004)](https://www.sciencedirect.com/science/article/pii/S030504830300152X).


### Instances for PMSP

Instance names are similar to PFSP: for ``20on4Rp50Rs50_1``, ``20`` refers to the number of tasks, ``4`` refers to the number of machines, ``1`` refers to instance id within ``20_4`` family. Other components of instance name describe parameters used on instance generation. Those information can be ignored.
The third paragraph of Section 4 of [Ezugwu (2019)](https://www.sciencedirect.com/science/article/pii/S0950705119300504) gives a short description of instance file format.

| Instance | \|_N_\| | \|_M_\| | BKS|
|----------|-------:|---------:|------:|
|[20on4Rp50Rs50_1  ](instances/pmsp/20on4Rp50Rs50_1.dat) | 20  | 4   |  527.80   ± 15.43   |
|[60on8Rp50Rs50_1  ](instances/pmsp/60on8Rp50Rs50_1.dat) | 60  | 8   |  820.00   ± 9.62    |
|[60on4Rp50Rs50_1  ](instances/pmsp/60on4Rp50Rs50_1.dat) | 60  | 4   |  1673.20  ± 43.67  |
|[80on8Rp50Rs50_1  ](instances/pmsp/80on8Rp50Rs50_1.dat) | 80  | 8   |  1089.00  ± 7.25   |
|[80on12Rp50Rs50_1 ](instances/pmsp/80on12Rp50Rs50_1.dat) | 80  | 12  |   711.60  ± 5.73   |
|[100on2Rp50Rs50_1 ](instances/pmsp/100on2Rp50Rs50_1.dat) | 100 | 2   |  5872.00  ± 33.32  |
|[100on6Rp50Rs50_1 ](instances/pmsp/100on6Rp50Rs50_1.dat) | 100 | 6   |  1858.40  ± 9.07   |
|[100on8Rp50Rs50_1 ](instances/pmsp/100on8Rp50Rs50_1.dat) | 100 | 8   |  1371.00  ± 12.10  |
|[120on12Rp50Rs50_1](instances/pmsp/120on12Rp50Rs50_1.dat) | 120 | 12  |   1087.80 ± 32.26 |
|[120on10Rp50Rs50_1](instances/pmsp/120on10Rp50Rs50_1.dat) | 120 | 10  |   1326.80 ± 13.46 |

__Note :__ Instances mirrored from [Scheduling Research Virtual Center](https://sites.wp.odu.edu/schedulingresearch/paper).

__Note 2:__ Best known solutions are presented in [Ezugwu (2019)](https://www.sciencedirect.com/science/article/pii/S0950705119300504).

__Note 3:__ A mathematical formulation of the problem can be found in [Ezugwu (2019)](https://www.sciencedirect.com/science/article/pii/S0950705119300504).


### Instances for TSPDL

TSPDL instances are adaptations from classic datasets for TSP. Instance names use the following convention: for ``bayg29_10_1``, ``bayg`` indicates the dataset to which the instance belongs, and``29`` indicates the number of vertices. The other informations can be ignored.
Instance format for ``bayg``, ``gr``, and ``ulysses`` is structured and self explanatory.
For ``KroA`` and ``pcb`` families, check the paper of [Reinelt (1991)](http://dx.doi.org/10.1287/ijoc.3.4.376).

| Instance | BKS (avg) | BKS (instance)|
|:---------|----------:|-----:|
|[bayg29_10_1    ](instances/tspdl/bayg29_10_1.dat)  |  1713.60     |  1610    |
|[bayg29_50_1    ](instances/tspdl/bayg29_50_1.dat)  |  2091.00     |  2105    |
|[gr17_25_1      ](instances/tspdl/gr17_25_1.dat)  |  2237.70       |  2265    |
|[gr48_10_1      ](instances/tspdl/gr48_10_1.dat)  |  6635.70       |  5046    |
|[gr48_25_1      ](instances/tspdl/gr48_25_1.dat)  |  5800.30       |  5161.65 |
|[KroA200_50_1   ](instances/tspdl/KroA200_50_1.dat)  |  30665.20   |  Unpublished  |
|[KroA200_75_1   ](instances/tspdl/KroA200_75_1.dat)  |  30896.10   |  Unpublished  |
|[pcb442_50_1    ](instances/tspdl/pcb442_50_1.dat)  |  59858.30    |  Unpublished  |
|[pcb442_75_1    ](instances/tspdl/pcb442_75_1.dat)  |  61010.10    |  Unpublished  |
|[Ulysses_22_50_1 ](instances/tspdl/ulysses22_50_1.dat)  |  8425.60  |  8290   |

__Note :__ Instances mirrored from [The TSPDL Lib](http://tspdl.jgr.no/).

__Note 2:__ Best known solutions are presented in [Todosijević et al. (2017)](https://link.springer.com/article/10.1007/s11590-014-0788-9). (See observation 4 below.)

__Note 3:__ A mathematical formulation of the problem can be found in [Rakke et al. (2012)](https://www.sciencedirect.com/science/article/pii/S0305048317300518).

__Note 4:__ The _BKS (avg)_ column presents the average best known solution to the entire instance family (bayg29_10, KroA200_50, and so forth). When available, the BKS of individual instances are presented in column _BKS (instance)_. Some individual results can also be found in [Battarra et al (2014)](https://www.sciencedirect.com/science/article/pii/S0377221713008655).

### Access to ILOG CPLEX optimization suite

Students and other academic members of Institute of Informatics can request a copy of the proprietary solver CPLEX, under __strictly academic conditions__. The software can be downloaded from through [OnTheHub](https://inf-ufrgs.onthehub.com/WebStore/Welcome.aspx) website. To request credentials to the OnTheHub, contact Library Chief Beatriz Haro.
