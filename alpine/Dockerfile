FROM alpine

RUN apk add build-base cmake coreutils curl unzip gettext-tiny-dev git ninja
RUN git clone --depth=1 https://github.com/neovim/neovim.git home/neovim

WORKDIR home/neovim
RUN make deps
RUN make
RUN make install
