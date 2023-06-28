FROM nvidia/cuda:11.1.1-cudnn8-devel-ubuntu20.04

RUN TZ=Europe/Bern && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt-get update && apt-get install -y \
  python3 \
  python3-pip \
  git \
  && rm -rf /var/lib/apt/lists/*

RUN pip3 install \
  torch \
  torchvision \
  torchaudio

RUN pip3 install deepcad

RUN git clone https://github.com/cabooster/DeepCAD-RT

