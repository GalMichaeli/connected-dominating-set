<h1 align="center">
    CDS4NX
    <br>
</h1>

<h3 align="center">
    Connected Dominating Set Algorithms with NetworkX
    <br>
</h3>

<h3 align="center">
    <a href="https://github.com/GalMichaeli">Gal Michaeli</a> •
    <a href="https://github.com/SergeyMashkin">Daniel Ben Shlush</a>
</h3>

<h4 align="center">Project A<br>Technion ECE 0440167 Winter 2025</h4>


## Overview
In this project we implement several connected dominating set (CDS) algorithms.
Namely, the first three algorithms in
[Guha & Khuller](https://scispace.com/pdf/approximation-algorithms-for-connected-dominating-sets-2slkc2r90s.pdf),
which find *some* CDS in general undirected graphs, and algorithms for finding *minimum* CDS for 
[interval graphs](https://scispace.com/papers/a-unified-approach-to-domination-problems-on-interval-graphs-et57c7pem9)
and
[permutation graphs](https://www.sciencedirect.com/science/article/abs/pii/S0196677484710212).
Furthermore, we enhance the first algorithm in
[Guha & Khuller](https://scispace.com/pdf/approximation-algorithms-for-connected-dominating-sets-2slkc2r90s.pdf)
with centrality metrics.


## Dependencies
| Library  | Version |
| -------- | ------- |
| `Python` | `3.11.12` |
| `networkx` | `3.4.2` |
| `numpy` | `2.0.2` |


## Usage
Download the notebook located in the ```code``` directory and run in Google Colaboratory.
Alternatively, you can directly
<a href="https://colab.research.google.com/github/GalMichaeli/connected-dominating-set/blob/main/code/connected-dominating-set.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

**Real-world graphs** can be transformed to NetworkX graphs in following way:
```
dolphins = nx.read_gml("dolphins.gml")
usair = nx.Graph(nx.read_pajek("USAir97.net"))
```

## Repository Organization
| Directory | Description |
|-----------|-------------|
| code | .ipynb file with implementations |
| csv | .csv files with data produced by running implemented algorithms on various graphs |
| real_world_graphs | .gml and .net graph files |


## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
