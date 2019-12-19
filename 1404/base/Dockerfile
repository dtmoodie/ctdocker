from ubuntu:14.04

RUN apt update && apt install wget build-essential cmake git -y
WORKDIR /workspace

RUN wget http://developer.download.nvidia.com/compute/cuda/repos/ubuntu1404/x86_64/cuda-repo-ubuntu1404_6.5-14_amd64.deb
RUN dpkg -i cuda-repo-ubuntu1404_6.5-14_amd64.deb

