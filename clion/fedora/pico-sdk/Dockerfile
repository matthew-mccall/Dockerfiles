FROM clion/fedora/cpp-env

RUN dnf install -y \
    git \
    gcc-arm-linux-gnu \
    arm-none-eabi-gcc-cs-c++ \
    arm-none-eabi-gcc-cs \
    arm-none-eabi-binutils \
    arm-none-eabi-newlib \
    boost-devel 

RUN git clone https://github.com/raspberrypi/pico-sdk.git --branch master
RUN git -C pico-sdk submodule update --init

ENV PICO_SDK_PATH=/pico-sdk
