FROM ubuntu:20.04
ENV TZ=Europe/Moscow
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone \
    && apt update && apt install -y \
    git \
    cmake \
    wget \
    software-properties-common \
    python3-pip \
    ninja-build \
    gcc-10 \
    g++-10 \
    clang \
    clang-tidy \
    && pip3 install --upgrade conan
