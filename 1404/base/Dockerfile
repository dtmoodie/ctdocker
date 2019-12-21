from ubuntu:14.04

RUN apt update && apt install wget build-essential cmake git -y
WORKDIR /workspace

RUN wget http://developer.download.nvidia.com/compute/cuda/repos/ubuntu1404/x86_64/cuda-repo-ubuntu1404_6.5-14_amd64.deb
RUN dpkg -i cuda-repo-ubuntu1404_6.5-14_amd64.deb
ENV DEBIAN_FRONTEND noninteractive
RUN apt update && apt install cuda-toolkit-6-5 -y
RUN wget https://github.com/Kitware/CMake/releases/download/v3.5.0/cmake-3.5.0-Linux-x86_64.sh && \
    chmod +x cmake-3.5.0-Linux-x86_64.sh && \
    ./cmake-3.5.0-Linux-x86_64.sh --prefix=/usr/local --exclude-subdir --skip-license && \
    rm ./cmake-3.5.0-Linux-x86_64.sh
