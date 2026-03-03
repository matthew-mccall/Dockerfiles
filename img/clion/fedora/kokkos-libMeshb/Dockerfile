FROM clion/fedora/cpp-env:1.0

RUN dnf install -y git git-lfs zlib-devel
RUN git lfs install

RUN git clone https://github.com/kokkos/kokkos.git
RUN cmake \
    -S kokkos \
    -B kokkos/build \
    -DCMAKE_INSTALL_PREFIX=/usr/local \
    -G Ninja
RUN cmake \
    --build kokkos/build \
    --target install

RUN git clone https://github.com/LoicMarechal/libMeshb.git
RUN cmake \
    -S libMeshb \
    -B libMeshb/build \
    -DCMAKE_INSTALL_PREFIX=/usr/local \
    -G Ninja
RUN cmake \
    --build libMeshb/build \
    --target install

RUN git clone https://github.com/UGAWG/parallel-adapt-results.git


ARG UID=1000
RUN useradd -m -u ${UID} -s /bin/bash mmccall
USER mmccall

RUN git config --global --add safe.directory "/tmp/omega_h"