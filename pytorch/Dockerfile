FROM pytorch/pytorch:1.3-cuda10.1-cudnn7-devel
RUN apt-get update
RUN apt-get install -y graphviz
ADD requirements.txt .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
WORKDIR /tmp

# docker build -t pytorch:jo .
# docker run -it -p 81:81 -p 5000:5000 -p 6006:6006 -p 8888:8888 --rm -v $PWD:/tmp pytorch:jo bash
# jupyter notebook --allow-root --ip=0.0.0.0