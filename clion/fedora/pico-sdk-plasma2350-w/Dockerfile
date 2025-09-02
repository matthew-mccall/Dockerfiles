FROM clion/fedora/arm-none-eabi-gcc

RUN dnf install -y \
    boost-devel

RUN git clone https://github.com/matthew-mccall/pico-sdk-plasma2350-w.git --branch master --depth 1 --recurse-submodules

ENV PICO_SDK_PATH=/pico-sdk-plasma2350-w