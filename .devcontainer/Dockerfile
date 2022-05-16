FROM ubuntu:22.04

ARG DEBIAN_FRONTEND=noninteractive

# Install base packages
RUN set -ex && \
	apt-get update && \
	apt-get install -y lsb-release wget software-properties-common

# Install clang toolchain version 14
RUN wget https://apt.llvm.org/llvm.sh &&\
	chmod +x llvm.sh && \
	./llvm.sh 14

# Install git, cmake, gdb
RUN set -ex && \
	apt-get update && \
	apt-get install -y git cmake gdb