FROM ubuntu:23.04@sha256:5a828e28de105c3d7821c4442f0f5d1c52dc16acf4999d5f31a3bc0f03f06edd

RUN export DEBIAN_FRONTEND=noninteractive && \
    apt-get update && \
    apt-get -y install \
        build-essential \
        curl \
        less \
        git \
        golang \
        gopls \
        delve \
        go-staticcheck

RUN go install honnef.co/go/tools/cmd/staticcheck@latest

CMD ["/bin/bash"]
