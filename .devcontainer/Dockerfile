# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.241.1/containers/rust/.devcontainer/base.Dockerfile

# [Choice] Debian OS version (use bullseye on local arm64/Apple Silicon): buster, bullseye
ARG VARIANT="buster"
FROM mcr.microsoft.com/vscode/devcontainers/rust:0-${VARIANT}


# [Optional] Uncomment this section to install additional packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install cmake g++ git wget curl build-essential libssl-dev python3-dev python3-pip 

# install zola
RUN mkdir -p /workspaces \ 
    && chmod 777 /workspaces \
    && cd /workspaces/ \
    && git clone https://github.com/getzola/zola \
    && cd zola \
    && cargo build --release \
    && cp target/release/zola /usr/local/bin

    #git clone https://github.com/amaranthosio/zolastrap.git
    
EXPOSE 1111:1111
