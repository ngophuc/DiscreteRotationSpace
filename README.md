# JMIV_2024_BijectiveDiscretizedRotations

Description
===========

BijectiveDiscretizedRotations studies the bijectivity of discrete rotations in 2D, with a particular focus on the combinatorial (hierarchical) structure of finite rotations of Z^2. 
This repository contains the C++ source code of two algorithms for building this structure described in the paper [Finite Rotations on Z2: A Hierarchical Framework for Bijectivity and Injectivity Analysis by N. Passat, P. Ngo, Y. Kenmochi in Journal of Mathematical Imaging and Vision, 2025](Comming soon). You can obtain a preprint
from [HAL](https://hal.science/hal-04945727v1) for free. 


Compilation
=============
1. Download or clone the repository.
2. ```cd <path to the cloned repository>```
3. ```mkdir build```
4. ```cmake .. -DDGtal_DIR=DGTAL_DIR [-DCMAKE_BUILD_TYPE=Release / Debug]```
5. ```make -j4```

NOTE : the implementation requires DGtal Libary (https://www.dgtal.org/) installed. 

Usage
================

There are two algorithms for building the structure of finite rotations of Z^2 :
- Bottom Up (algorithm 1) -> program name: AlgoBottomUp
- Top down (algorithm 2) -> program name: AlgoTopDown

The program takes as input an interger coresponding to the size of the Eucliden ball and produces as output a saliency map XXXX.pgm, which is the visualization of the hierarchy after performing the hierarchical graph based segmentation from a non increasing edge observation attribute of the input image.

To execute the program:

./ProgramName INT


./AlgoBottomUp

./AlgoTopDown

