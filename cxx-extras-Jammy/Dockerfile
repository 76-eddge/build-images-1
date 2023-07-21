FROM ubuntu:jammy AS deploy

RUN apt-get update && apt-get install -y build-essential cmake unzip curl wget tar sqlite gcovr

# Compile Boost 1.80
WORKDIR /
RUN wget https://boostorg.jfrog.io/artifactory/main/release/1.80.0/source/boost_1_80_0.tar.gz
RUN tar -xzf boost_1_80_0.tar.gz
WORKDIR /boost_1_80_0
RUN ./bootstrap.sh
RUN ./b2 -j8 install
WORKDIR /
RUN rm -rf boost_1_80_0
