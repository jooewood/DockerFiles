FROM auroraywood/aidd:ubuntu20.04-conda-base


RUN conda create -c rdkit -n rdkit_pytorch rdkit -y
RUN echo "conda activate rdkit_pytorch" >> ~/.bashrc
ENV PATH /opt/conda/envs/rdkit_pytorch/bin:$PATH


RUN /bin/bash -c "source activate rdkit_pytorch && conda install pytorch torchvision torchaudio cudatoolkit=11.1 -c pytorch-lts -c nvidia -y"
ENV CONDA_DEFAULT_ENV $rdkit_pytorch