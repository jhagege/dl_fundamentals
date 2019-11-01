FROM tensorflow/tensorflow:1.15.0-gpu-py3-jupyter
RUN apt-get update
RUN curl -sL https://deb.nodesource.com/setup_13.x | bash -
RUN apt-get install -y vim wget nodejs
ADD requirements.txt .
RUN pip install --upgrade pip && \
    pip install -r requirements.txt
WORKDIR /tmp

# docker run -it -p 81:81 -p 5000:5000 -p 8888:8888 --rm -v $PWD:/tmp tensorflow:jo bash
# jupyter notebook --allow-root --ip=0.0.0.0