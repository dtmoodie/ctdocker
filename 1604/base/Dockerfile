from ubuntu:16.04

RUN apt update && apt install wget build-essential cmake git -y
WORKDIR /workspace

RUN wget https://developer.nvidia.com/compute/cuda/9.2/Prod2/local_installers/cuda-repo-ubuntu1604-9-2-local_9.2.148-1_amd64
RUN sudo dpkg -i cuda-repo-ubuntu1604-9-2-local_9.2.148-1_amd64
RUN sudo apt-key add /var/cuda-repo-9.2/7fa2af80.pub
RUN sudo apt-get update
RUN sudo apt-get install cuda

