# 2023.0286
## An Exact Algorithm for Multicommodity Network Design under Stochastic Interdictions

This repository contains different variants of branch-and-Benders-cut algorithm with acceleration techniques presented in "An Exact Algorithm for Multicommodity Network Design under Stochastic Interdictions".

This archive is distributed in association with the [INFORMS Journal on Computing](https://pubsonline.informs.org/journal/ijoc) under the [MIT License](https://github.com/shabnamvaziri/IJOC-paper/blob/main/LICENSE.txt).

## Cite
To cite the contents of this repository, please cite both the paper and this repo, using their respective DOIs.

http://doi.org/10.1287/ijoc.2023.0286

http://doi.org/10.1287/ijoc.2023.0286.cd

Below is the BibTex for citing this snapshot of the repository.

```bibtex
@misc{Vaziri2024,
  author =        {Vaziri, Shabnam Mahmoudzadeh and Kuzgunkaya, Onur and Vidyarthi, Navneet},
  publisher =     {INFORMS Journal on Computing},
  title =         {{An Exact Algorithm for Multicommodity Network Design under Stochastic Interdictions}},
  year =          {2024},
  doi =           {10.1287/ijoc.2023.0286.cd},
  url =           {https://github.com/INFORMSJoC/2023.0286},
  note =          {Available for download at https://github.com/INFORMSJoC/2023.0286},
}
```
## Description
This repository contains 5 folders, each for one variant of the branch-and-Benders-cut algorithm presented in the paper as follows.

- BBC1: Multicut reformulation
- BBC2: Multicut reformulation with penalty reformulation
- BBC3: Multicut reformulation with Pareto-optimal cuts
- BBC4: Multicut reformulation with supervalid and valid inequalities
- BBC5: Multicut reformulation with all the acceleration techniques 

Please note that for using the codes in Visual Studio, you should change the time function to clock(). The current time fucntion gettimeofday(&stop, NULL) is for Linux.

## Building
To use the code, you need CPLEX 22.1.0. To use other versions of CPLEX, please modify the Makefile and def.h with your CPLEX version.

To run e.g. BBC2 in Linux:

```
make

./BBCPenaltymulti Input.txt
```

## Results
All detailed results are available in the [Results](https://github.com/shabnamvaziri/IJOC-paper/tree/main/Results) folder.
