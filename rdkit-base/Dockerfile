FROM auroraywood/aidd:ubuntu20.04-conda-base


RUN conda create -c rdkit -n rdkit rdkit -y

RUN echo "conda activate rdkit" >> ~/.bashrc
ENV PATH /opt/conda/envs/rdkit/bin:$PATH
ENV CONDA_DEFAULT_ENV $rdkit
RUN python -c "import rdkit; print(rdkit.__version__)"