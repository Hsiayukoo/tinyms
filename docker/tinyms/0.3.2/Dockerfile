ARG BASE_CONTAINER=swr.cn-south-1.myhuaweicloud.com/mindspore/mindspore-cpu:1.6.0
FROM $BASE_CONTAINER

LABEL MAINTAINER="TinyMS Authors"

# Install base tools
RUN apt-get update
# Install opencv dependencies software
RUN apt-get install libglib2.0-dev libsm6 libxrender1 libgl1-mesa-glx -y

# Install TinyMS cpu whl package
RUN pip install --upgrade -i https://pypi.mirrors.ustc.edu.cn/simple pip && pip install --no-cache-dir -i https://pypi.mirrors.ustc.edu.cn/simple tinyms==0.3.2
