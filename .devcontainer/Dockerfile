FROM mcr.microsoft.com/devcontainers/cpp:ubuntu-22.04

# Install C development toolchain, debuggers, and static analysis tools
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
       build-essential \
       gdb \
       valgrind \
       clang-format \
       cppcheck \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
       build-essential \
       gdb \
       git-lfs \
    && apt-get clean && rm -rf /var/lib/apt/lists/*