# InteractiveGraphRepair
Interactive graph repair for neighborhood constraints with simulated users on both synthetic and real-world data

# Paper Abstract

# Reproducibility guidelines

All the necessary material is included. Jupyter notebooks can be run independetly as previous checkpoints are provided.
Some cells might take a while to run but all terminate in reasonable time (~few hours) on a 16G main memory laptop with intel i7 processor.

The code is produced with the following environment:
- Python 3.8.11
- matplotlib 3.5.1
- networkx 2.8.8
- pandas 1.4.2
- numpy 1.22.3
- seaborn 0.11.2
- bs4 4.10

# Content Description

This repository contains the necessary code and data to run experiements simulating user repair of graph data under Neighborhood Constraints.
Most of the implementation is included in `igr.py`.
The code is presented as seperate jupyter notebooks with distinct goals. The raw data is kept in the `data` directory. All data can be freely accessed online (details below).
The `temp` directory holds various checkpoints.

### Synthetic Dataset
Creation of the Synthetic dataset used in the experiments. It creates labeled graphs and constraint sets and injects noise to have a (instance, ground truth) pairs.

### Restaurants
Reads the restaurant data and creates the Restaurant dataset used in the experiments.

### Sepsis Process Mining
Reproduce the result of the process mining task done in 
[this](https://www.researchgate.net/publication/316880149_Analyzing_the_Trajectories_of_Patients_with_Sepsis_using_Process_Mining) 
paper and creates the Sepsis dataset used for the experiments.

### Coauthor
Read the dblp and citeseerx data and creates the coauthor dataset used in experiments.

### Experiments and analysis
Merges all datasets, computes metrics and produces results and graphs.

### Time to next question
Quick timing experiment to confirm the time to produce a new question is of the order of micro-seconds.

# Footnote
This work is produced by Paul Juillard as part of their EPFL master's internship supervised by Angela Bonifati and Andrea Mauri at Inria Lab in Lyon University
