# QTLNetwork-MP

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Citation

Please cite our manuscript if you use our software.

```
Agrawal A, Chiu AM, Le M, Halperin E, Sankararaman S (2020) Scalable probabilistic PCA for large-scale genetic variation data. PLOS Genetics 16(5): e1008773. https://doi.org/10.1371/journal.pgen.1008773
```

## Built With
The following packages are required on a Linux machine to compile and use the software package.

```
g++
cmake
make
```

### Installing
Installing QTLNetwork-MP is fairly simple. Just issue the following commands on a Linux machine

```
git clone https://github.com/Zhutn/QTXNetwork4.0.git
cd QTXNetwork4.0
cd build
```

### Run with example data

**Options for QTLNetwork-MP**

* `--map` genetic map for QTL mapping.

* `--txt` txt for QTL mapping.

* `--threads` thread number (default, maximum).

* `--test-window` The size of testing window for background control. (default, 10.0 cM).

* `--scan-step` The genetic distance of step for QTL mapping. (default, 1.0 cM).

* `--only-1D` 1D scan only (--only-1D "any integer"). (default, False).

* `--output-1D` Output the results of HendersonIII F values for 1D scan (--output-1D "any integer"). (default, False).

**Examples for QTLNetwork-MP**

```
./QTXNetwork --map ../example/SimF2.map --txt ../example/SimF2.txt --QTX 0 --out SimF2.pre
./QTXNetwork --map ../example/Sim_fourway_1.map --txt ../example/Sim_fourway_1.txt --QTX 0 --out sorghum.pre

```
```
