FROM clion/fedora/arm-none-eabi-gcc

RUN dnf install -y \
    boost-devel 

RUN git clone https://github.com/raspberrypi/pico-sdk.git --branch master
RUN git -C pico-sdk submodule update --init

ENV PICO_SDK_PATH=/pico-sdk
