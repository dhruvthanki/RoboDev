# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.187.0/containers/cpp/.devcontainer/base.Dockerfile

# [Choice] Debian / Ubuntu version: debian-10, debian-9, ubuntu-20.04, ubuntu-18.04
ARG VARIANT="buster"
FROM mcr.microsoft.com/vscode/devcontainers/cpp:0-${VARIANT}

# [Optional] Uncomment this section to install additional packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends build-essential pkg-config cmake git wget curl tar unzip

# # Eigen
# ARG EIGEN3_VERSION=3.3.7
# WORKDIR /tmp
# RUN set -x && \
#   wget -q http://bitbucket.org/eigen/eigen/get/${EIGEN3_VERSION}.tar.bz2 && \
#   tar xf ${EIGEN3_VERSION}.tar.bz2 && \
#   rm -rf ${EIGEN3_VERSION}.tar.bz2 && \
#   mv eigen-eigen-* eigen-${EIGEN3_VERSION} && \
#   cd eigen-${EIGEN3_VERSION} && \
#   mkdir -p build && \
#   cd build && \
#   cmake \
#     -DCMAKE_BUILD_TYPE=Release \
#     -DCMAKE_INSTALL_PREFIX=${CMAKE_INSTALL_PREFIX} \
#     .. && \
#   make -j${NUM_THREADS} && \
#   make install && \
#   cd /tmp && \
#   rm -rf *
# ENV Eigen3_DIR=${CMAKE_INSTALL_PREFIX}/share/eigen3/cmake

# CMD ["./src/main.exe"]