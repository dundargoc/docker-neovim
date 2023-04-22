FROM centos

RUN sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*
RUN sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*
RUN dnf -y install cmake gcc make unzip gettext curl git
RUN git clone --depth=1 https://github.com/neovim/neovim.git home/neovim

WORKDIR home/neovim
RUN make deps
RUN make
RUN make install
