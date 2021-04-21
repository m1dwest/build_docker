FROM archlinux

RUN pacman -Syu --noconfirm \
    && pacman -S --noconfirm \
        gcc \
        make \
        git \
        cmake \
        python-pip \
        ninja \
        clang \
        libc++ \
        libc++abi \
    && pip install --upgrade conan

