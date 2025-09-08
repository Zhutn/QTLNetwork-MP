# QTLNetwork-MP

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Citation

Please cite our manuscript if you use our software.

```
Tianneng Zhu (2025) QTLNetowrk-MP: An Epistatic Mapping Method of Complex Traits in Multiparent Advanced Generation Intercross (MAGIC) Populations.
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
git clone git@github.com:Zhutn/QTLNetwork-MP.git
cd QTLNetwork-MP
chmod 755 QTXNetwork
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
./QTXNetwork --map ./example/SimF2.map --txt ./example/SimF2.txt --out SimF2.pre
./QTXNetwork --map ./example/Sim_fourway_1.map --txt ./example/Sim_fourway_1.txt --out sorghum.pre

```
```
