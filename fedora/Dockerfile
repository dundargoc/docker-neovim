FROM fedora

RUN yum -y install ninja-build cmake gcc make unzip gettext curl git glibc-gconv-extra
RUN git clone --depth=1 https://github.com/neovim/neovim.git home/neovim

WORKDIR home/neovim
RUN make deps
RUN make
RUN make install
