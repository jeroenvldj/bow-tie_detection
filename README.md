# Bow-tie detection
Bow-tie structure detection in directed networks

&nbsp;&nbsp;
![Python](https://img.shields.io/badge/python-3.5%2B-orange.svg)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A python implementation for the detection of a bow-tie structure in a directed network, following the definition as in: 
["Bow-tie Decomposition in Directed Graphs" - Yang et al. IEEE (2011)](https://www.researchgate.net/profile/Lily_Popova_Zhuhadar/publication/252027520_Bow-tie_decomposition_in_directed_graphs/links/5b3477580f7e9b0df5d2987f/Bow-tie-decomposition-in-directed-graphs.pdf)

## Example - Running the code
The provided `jupyter notebook` contains a working example.
  1. Loading a directed network/graph, either as the corresponding adjacency matrix in `numpy.array` format or as a `NetworkX.DiGraph`
```python
G = nx.DiGraph(nx.scale_free_graph(16, seed=14))
```
  2. Running the detection function
```python
S, IN, OUT, TUBES, INTENDRILS, OUTTENDRILS, OTHER = get_bowtie_components(graph=G)
```

<p align="center"><img width=40% src="https://github.com/jeroenvldj/bow-tie_detection/blob/master/bow-tie_partitioning_example.png"></p>

