# QTLNetwork-MP

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.


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

* `--map` genetic map for QTL or genotype for QTS.

* `--txt` txt for QTL or phenotype for QTS.

* `--QTX` 0 for QTL mapping or 1 for QTS (default, QTL).

* `--threads` thread number (default, maximum).

* `--test-window` The size of testing window for background control. (default, 10.0 cM).

* `--scan-step` The genetic distance of step for QTL mapping. (default, 1.0 cM).

* `--only-1D` 1D scan only (--only-1D "any integer"). (default, False).

* `--output-1D` Output the results of HendersonIII F values for 1D scan (--output-1D "any integer"). (default, False).

**Examples for QTLNetwork-MP**

```
./QTXNetwork --map ../example/SimF2.map --txt ../example/SimF2.txt --QTX 0 --out SimF2.pre
./QTXNetwork --map ../example/sorghum.map --txt ../example/sorghum.txt --QTX 0 --out sorghum.pre
./QTXNetwork --map ../example/SimF2_600.Gen --txt ../example/SimF2_600.Phe --QTX 1 --out SimF2_600.pre
./QTXNetwork --map ../example/0pca.Girth18.gen --txt ../example/0pca.Girth18.phe --QTX 1 --out 0pca.Girth18.pre

```
```
