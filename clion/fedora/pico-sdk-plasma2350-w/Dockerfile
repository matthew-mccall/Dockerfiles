FROM clion/fedora/cpp-env

RUN dnf install -y \
    git \
    gcc-arm-linux-gnu \
    arm-none-eabi-gcc-cs-c++ \
    arm-none-eabi-gcc-cs \
    arm-none-eabi-binutils \
    arm-none-eabi-newlib \
    boost-devel

RUN git clone https://github.com/matthew-mccall/pico-sdk-plasma2350-w.git --branch master --depth 1 --recurse-submodules

ENV PICO_SDK_PATH=/pico-sdk-plasma2350-w