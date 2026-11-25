FROM mcr.microsoft.com/devcontainers/base:ubuntu24.04
RUN export DEBIAN_FRONTEND=noninteractive \
    && dpkg --add-architecture i386 \
    && apt-get update \
    && apt-get install -y --no-install-recommends \
        bison \
        clang-format-19 \
        flex \
        g++ \
        gcc-arm-none-eabi \
        git \
        libc6:i386 \
        libpng-dev \
        make \
        nasm \
        ninja-build \
        pkg-config \
        python3 \
        wget \
        xz-utils \
    && ln -s /usr/bin/clang-format-19 /usr/local/bin/clang-format \
    && rm -rf /var/lib/apt/lists/*
