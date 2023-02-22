# Quantum random walk simulation

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TendTo/Quantum-random-walk-simulation/main?filepath=QuantumWalk.ipynb)

## Use

To run the Jupyter notebook locally, you need to ensure the following dependencies are installed:

- [python](https://www.python.org/downloads/)
- [juptyer](https://jupyter.org/install)
- [qiskit](https://qiskit.org/documentation/getting_started.html)
- [qiskit\[visualization\]](https://qiskit.org/documentation/getting_started.html)
- [pygraphviz](https://pygraphviz.github.io/documentation/stable/install.html)

### Slides

To transform the Jupyter notebook into a slideshow, you need to install [RISE](https://rise.readthedocs.io/en/stable/installation.html) and enable it in the Jupyter notebook.

## Docker

Another option is to use the Docker image provided. You can either build it yourself or pull it from Docker Hub.

### Build

```shell
docker build -t tendto/quantum:quantum-walk .
```

### Pull

```shell
docker pull tendto/quantum:quantum-walk
```

### Run

```shell
docker run -it --rm -p 8888:8888 -e DOCKER_STACKS_JUPYTER_CMD=notebook tendto/quantum:quantum-walk
```

You can then access the Jupyter notebook at [http://127.0.0.1:8888](http://127.0.0.1:8888), using the token provided in the terminal.

## References

- [Quantum Walk Search Algorithm](https://qiskit.org/textbook/ch-algorithms/quantum-walk-search-algorithm.html)
- [An Insight Into: Quantum Random Walks](https://bayesianbrad.github.io/assets/publications/2014_thesis/paper.pdf)
- [Quantum Walks and Search Algorithms](http://ndl.ethernet.edu.et/bitstream/123456789/73178/1/277.pdf)
- [Quantum Walk](https://quantumai.google/cirq/experiments/quantum_walks)
