FROM alpine:3.8

RUN apk add build-base cmake coreutils curl unzip git ninja gettext-dev
RUN git clone --depth=1 https://github.com/neovim/neovim.git home/neovim

WORKDIR home/neovim
RUN make deps
RUN make
RUN make install
