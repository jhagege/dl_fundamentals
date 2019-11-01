FROM pytorch/pytorch:0.4.1-cuda9-cudnn7-devel
RUN apt-get update
ADD requirements.txt .
RUN pip install -r requirements.txt


# docker build -t pytorch:jo .
# docker run -it -p 81:81 -p 5000:5000 -p 8888:8888 --rm -v $PWD:/tmp pytorch:jo bash
# jupyter notebook --allow-root --ip=0.0.0.0