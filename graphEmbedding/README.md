This project implemented DeepWalk and Node2Vec using GSQL.
```
[1] Perozzi, Bryan, Rami Al-Rfou, and Steven Skiena. "Deepwalk: Online learning of social representations." Proceedings of the 20th ACM SIGKDD international conference on Knowledge discovery and data mining. ACM, 2014.
[2] Grover, Aditya, and Jure Leskovec. "node2vec: Scalable feature learning for networks." Proceedings of the 22nd ACM SIGKDD international conference on Knowledge discovery and data mining. ACM, 2016.
```


Usage:
1. Add User-Defined Functions into TigerGraph Platform. See details in User-Defined-Functions folder 
2. Install graph data like Karate. See details in Benchmark-data folder
3. Install deepWalk.gsql query and randomWalk.gsql query
4. Install node2vec.gsql query

Sample randomWalk/deepWalk output:

```
860 5705 3968 5705 996 667 7127 4839 5402 8376 9969 9280 7533 9280 9808 739 3354 2928 982 1464 1805 867 958 1263 5705 3084 2156 9526 9143 5241 3644 1047 9674 3415 4374 10091 446 7515 7614 8315 1273 1226 6237 7373 5920 6872 6058 750 7103 7815 26 867 2499 6034 8615 8470 3224 3785 1745 2709 3339 2197 7010 4335 6574 3526 5159 5130 296 5671 4669 7701 5256 8982 1020 1832 3262 1557 3607 6660 8868 

1001 1196 6058 6485 4805 1391 9636 9890 4948 4851 3266 6427 6977 6986 4389 6566 7205 8460 6115 8157 4478 8302 6724 7623 7075 7189 8293 6802 7932 8425 6030 9641 7892 5133 10303 5446 2999 1456 2182 1456 4862 5924 3561 5510 3198 5934 4839 592 1136 1423 5681 8733 3323 4218 9465 4374 6084 8775 1127 1085 1127 5705 5918 2175 2228 474 3914 3315 1418 5681 5003 5843 5984 4407 2115 667 6432 9937 9396 8196 8859 
```

Train node2vec:
```
node2vec(128,"/home/tigergraph/randomWalk_blog.txt","/home/tigergraph/vectors_randomWalk_blog.txt");
```

