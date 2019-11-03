FROM pytorch/pytorch:1.1.0-cuda10.0-cudnn7.5-devel
RUN apt-get update
ADD requirements.txt .
RUN pip install --upgrade pip && \
    pip install -r requirements.txt
WORKDIR /tmp

# docker build -t pytorch:jo .
# docker run -it -p 81:81 -p 5000:5000 -p 8888:8888 --rm -v $PWD:/tmp pytorch:jo bash
# jupyter notebook --allow-root --ip=0.0.0.0