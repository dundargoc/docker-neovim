FROM opensuse/tumbleweed:latest

RUN zypper --non-interactive install ninja cmake gcc-c++ gettext-tools curl git unzip
RUN git clone https://github.com/neovim/neovim.git home/neovim

WORKDIR home/neovim
# RUN make
# RUN make install
