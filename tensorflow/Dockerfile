FROM tensorflow/tensorflow:latest-gpu-py3-jupyter
RUN apt-get update
# RUN curl -sL https://deb.nodesource.com/setup_13.x | bash -
RUN apt-get install -y vim wget
ADD requirements.txt .
RUN pip install --upgrade pip && \
    pip install -r requirements.txt
WORKDIR /tmp

# docker build -t tensorflow:jo .
# docker run -it -p 81:81 -p 5000:5000 -p 8888:8888 --rm -v $PWD:/tmp tensorflow:jo bash
# jupyter notebook --allow-root --ip=0.0.0.0