FROM auroraywood/aidd:ubuntu20.04-rdkit-pytorch1.8.2-py37-cuda11-conda-base


RUN /bin/bash -c "source activate rdkit_pytorch && conda install -c conda-forge pytorch-lightning -y"
RUN python -V