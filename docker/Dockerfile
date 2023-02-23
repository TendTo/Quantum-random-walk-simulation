FROM jupyter/datascience-notebook:85f615d5cafa

ENV DOCKER_STACKS_JUPYTER_CMD=notebook
EXPOSE 8888

WORKDIR /home/jovyan/work

RUN conda install -c conda-forge -y rise
RUN conda install -c conda-forge -y jupyter_contrib_nbextensions pygraphviz
RUN pip3 install qiskit qiskit[visualization]
RUN jupyter-nbextension enable splitcell/splitcell
RUN jupyter-nbextension enable hide_input/main

COPY QuantumWalk.ipynb .
