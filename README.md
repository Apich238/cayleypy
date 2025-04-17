# CaleyPy
Library for studying Cayley graphs and Schreier coset graphs.

## Overview

This is a library for studying
[Schreier coset graphs](https://en.wikipedia.org/wiki/Schreier_coset_graph)
and [Caley graphs](https://en.wikipedia.org/wiki/Cayley_graph).

This what we plan to support:
* BFS from given state (growth function, adjacency matrix, last layers).
* Efficient path finding (beam search).
* Random walk generation.
* Library of graphs and generators (LRX, TopSpin, Rubik Cubes, wreath, globe etc., 
    see [here](https://www.kaggle.com/code/ivankolt/generation-of-incidence-mtx-pancake)).
* Efficient computing on CPU, GPU, TPU (with JAX), usable on Kaggle.
* Library of datasets with solutions to some problems (e.g. growth functions like
    [here](https://www.kaggle.com/code/fedimser/bfs-for-binary-string-permutations)).



## Development

To start development, clone the repository, then run:

```
pip install -r requirements.txt
pip install -r requirements-dev.txt
```

Before commiting, run these checks:
```
./lint.sh
pytest 
```


## Credits

The initial code for this library is based on [cayleypy](https://github.com/iKolt/cayleypy)
by [Ivan Koltsov](https://github.com/iKolt), which is itself based on code by 
[Alexander Chervov](https://github.com/chervov) and 
[Kirill Khoruzhii](https://github.com/k1242).

Also, code from the following Kaggle notebooks was used:
* https://www.kaggle.com/code/ivankolt/generation-of-incidence-mtx-pancake (advanced BFS).
* https://www.kaggle.com/code/avm888/cayleypy-growth-function.
* https://www.kaggle.com/code/avm888/jax-version-cayleypy (how to use JAX).
* https://www.kaggle.com/code/fedimser/bfs-for-binary-string-permutations (bit operations).

