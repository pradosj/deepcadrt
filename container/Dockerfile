FROM nvidia/cuda:11.1.1-runtime-ubuntu18.04

RUN apt-get update && apt-get install -y \
  python3 \
  python3-pip \
  git \
  && rm -rf /var/lib/apt/lists/*
  
RUN pip3 install \
  torch==1.8.0+cu111 \
  torchvision==0.9.0+cu111 \
  torchaudio==0.8.0 \
  -f https://download.pytorch.org/whl/torch_stable.html

#RUN pip3 install deepcad


