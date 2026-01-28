FROM mcr.microsoft.com/vscode/devcontainers/miniconda:0-3

COPY yarn-archive-keyring.gpg /usr/share/keyrings/yarn-archive-keyring.gpg
RUN chmod a+r /usr/share/keyrings/yarn-archive-keyring.gpg
COPY sample_keys.cfg keys.cfg
RUN conda install -y -c conda-forge uv && conda clean -afy 
