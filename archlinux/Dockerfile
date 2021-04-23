FROM archlinux

RUN pacman -Syu --noconfirm \
    && pacman -S --noconfirm \
        gcc \
        make \
        ccache \
        wget \
        qt5 \
        git \
        cmake \
        python-pip \
        ninja \
        clang \
        libc++ \
        libc++abi \
    && pip install --upgrade conan numpy

RUN mkdir /fbx_sdk && cd $_ \
    && wget https://www.autodesk.com/content/dam/autodesk/www/adn/fbx/2020-2/fbx20202_fbxsdk_linux.tar.gz \
    && tar xfz fbx20202_fbxsdk_linux.tar.gz \
    && yes yes | ./fbx20202_fbxsdk_linux .

