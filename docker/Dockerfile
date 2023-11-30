FROM ghcr.io/steamdeckhomebrew/holo-base:latest

RUN pacman -Syu --noconfirm
RUN pacman -S --noconfirm meson pkgconf glslang libx11 spirv-headers vulkan-headers lib32-libx11 lib32-glibc lib32-gcc-libs

WORKDIR /workdir
ADD . /workdir

ENTRYPOINT [ "/docker/build" ]