FROM jupyter/scipy-notebook 

USER root 

# python 3 environment is named root 
RUN conda install --yes --name root spacy pymongo
# install libraries via pip using bash and activating respective environment 
RUN ["bash", "-c", "source activate root && pip install twitter"]
RUN python -m spacy download en 

USER jovyan