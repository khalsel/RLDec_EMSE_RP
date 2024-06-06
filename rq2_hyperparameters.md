## Mono2Micro: 
We used different values of the “number of clusters” hyper parameter:
- For petcllinic, roller, jpetstore-6, partsunlimitedmrp and 7ep-demo”: [5, 8, 10, 12, 14, 16, 18, 20]
-  the rest of the projects: we used the decompositions presented in their paper

## CoGCN: 
We used different values of the “number of partitions” hyper parameter: [6, 8, 10, 12, 14, 16, 18, 20]

## TopicDecomp: 
By default, TopicDecomp’s implementation  generates multiple results with different resolution parameter values. We used its default configuration.

## MSExtractor: 
We ran 50 iterations of random search across different the following hyperparameters intervals:
- max number of clusters= random integer between (√N, 3 * √N) N is the number of classes
- number of generations = [100, 300, 500, 1000, 2000]
- population size = [50, 100, 200]
- crossover probability = uniform distribution with (loc=0, scale=1)
- mutation probability = uniform distribution with (loc=0, scale=1)
- attribute mutation probability = uniform distribution with (loc=0, scale=0.2)

## HyDec: 
We used a grid search across the following hyper-parameter ranges:
- dynamic analysis epsilon:  range(0.05, 1, 0.1)
- dynamic analysis similarity: [“call”, “cousage”]
- static analysis epsilon:  range(0.05, 1, 0.1)
- structural analysis similarity: [“call”, “cousage”]
- semantic analysis aggregation: [“mean”, “sum”]
- min samples: [2, 3]
- epsilon step: [0.01, 0.05, 0.1]
