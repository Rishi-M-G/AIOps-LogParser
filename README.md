# AIOps-LogParser
This repository is a part of COEN691 - Artificial Intelligence for Software Systems Operations course instructed by Professor Wahab Hamou-Lhadj, PhD.


## AEL

AEL (Abstracting Execution Logs) is one of the state-of-the-art log parsing approaches, which comprises four steps: anonymize, tokenize, categorize, and reconcile. In particular, in the reconcile step, the original algorithm merges events that have only a different token. However, this process cannot handle the cases where one single template multiple different parameter tokens. To improve the generability of this algorithm, we use a parameter merge_percent to set the percentage of different tokens when merging two events.

Read more information about AEL from the following paper:

+ Zhen Ming Jiang, Ahmed E. Hassan, Gilbert Hamann, Parminder Flora. [An Automated Approach for Abstracting Execution Logs to Execution Events](http://www.cse.yorku.ca/~zmjiang/publications/jsme2008.pdf), *Journal of Software Maintenance and Evolution: Research and Practice (JSME)*, 2008.




Run the following scripts to start the demo:

```
python demo.py
```

Run the following scripts to execute the benchmark:

```
python benchmark.py
```

### Benchmark

Running the benchmark script on Loghub_2k datasets, you could obtain the following results.

# Drain

Drain is an online log parser that can parse logs into structured events in a streaming and timely manner. It employs a parse tree with fixed depth to guide the log group search process, which effectively avoids constructing a very deep and unbalanced tree. 

Read more information about Drain from the following paper:

+ Pinjia He, Jieming Zhu, Zibin Zheng, and Michael R. Lyu. [Drain: An Online Log Parsing Approach with Fixed Depth Tree](http://jiemingzhu.github.io/pub/pjhe_icws2017.pdf), *Proceedings of the 24th International Conference on Web Services (ICWS)*, 2017.


### Running

The code has been tested in the following enviornment:
+ python 3.7.6
+ regex 2022.3.2
+ pandas 1.0.1
+ numpy 1.18.1
+ scipy 1.4.1

Run the following scripts to start the demo:

```
python demo.py
```

Run the following scripts to execute the benchmark:

```
python benchmark.py
```

### Benchmark

Running the benchmark script on Loghub_2k datasets, you could obtain the following results.
