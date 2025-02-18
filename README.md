# JMIV_2024_DiscreteRotationSpace

Description
===========

BijectiveDiscretizedRotations studies the bijectivity of discrete rotations in 2D, with a particular focus on the combinatorial (hierarchical) structure of finite rotations of Z^2. 
This repository contains the C++ source code of two algorithms for building this structure described in the paper [Finite Rotations on Z2: A Hierarchical Framework for Bijectivity and Injectivity Analysis by N. Passat, P. Ngo, Y. Kenmochi in Journal of Mathematical Imaging and Vision, 2025](Comming soon). You can obtain a preprint
from [HAL](https://hal.science/hal-04945727v1) for free. 

Dependencies
=============
- DGtal (https://dgtal.org/)
- GMP (https://gmplib.org/)

Compilation
=============
1. Download or clone the repository.
2. ```cd <path to the cloned repository>```
3. ```mkdir build```
4. ```cmake .. -DDGtal_DIR=DGTAL_DIR [-DCMAKE_BUILD_TYPE=Release / Debug]```
5. ```make -j4```

# Running command
There are two algorithms for building the structure of finite rotations of Z^2 :
- Bottom Up (algorithm 1) -> program_name: AlgoBottomUp
- Top down (algorithm 2) -> program_name: AlgoTopDown

  
```sh
./program_name -h

Build the tree structure of finite rotations of Z^2.
 Typical use example:
 	 program_name -r 10

Usage: ./program_name [OPTIONS]

Options:
  -h,--help                             Print this help message and exit
  -r,--radius INT=5                     Square of radius of the euclien ball (default 5)
```

Examples of valid commands
================

```sh
./AlgoBottomUp
./AlgoBottomUp -r 20
./AlgoBottomUp --radius 50
./AlgoTopDown
./AlgoTopDown -r 30
./AlgoTopDown --radius 40
```
