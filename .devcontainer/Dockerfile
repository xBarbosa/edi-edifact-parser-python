# Use a imagem base do Python 3.12
FROM mcr.microsoft.com/devcontainers/python:3.12-bullseye

# Instale o pacote smbclient para montar compartilhamentos SMB
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends smbclient

# Crie o diretório de montagem
#RUN mkdir -p /mnt/z

# Instale o Jupyter Notebook
RUN pip install notebook

# Instale as dependências do seu projeto (se houver)
# COPY requirements.txt /tmp/pip-tmp/
# RUN pip install --no-cache-dir --upgrade -r /tmp/pip-tmp/requirements.txt