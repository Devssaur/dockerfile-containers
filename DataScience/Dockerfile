#imagem com jupyter notebook e algumas bibliotecas

FROM python:3.8-slim-buster

RUN mkdir -p /home/notebook 
WORKDIR /home/notebook

RUN pip install numpy \
                pandas \
                scikit-learn \
                tensorflow \
                seaborn \
                jupyter \
                notebook
EXPOSE 8888

#inicializa jupyter
ENTRYPOINT [ "jupyter", "notebook", "--ip=0.0.0.0","--allow-root", "--no-browser"]
