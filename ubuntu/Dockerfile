FROM ubuntu

RUN apt-get update && apt-get install -y ninja-build gettext cmake unzip curl git
RUN git clone --depth=1 https://github.com/neovim/neovim.git home/neovim

WORKDIR home/neovim
RUN make deps
RUN make
RUN make install
