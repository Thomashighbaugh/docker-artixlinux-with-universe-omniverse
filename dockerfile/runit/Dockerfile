FROM thighbaugh/artixlinux-with-universe-omniverse-base:latest
RUN pacman-key --init && pacman-key --populate artix 
RUN pacman --noconfirm -Syu --overwrite '*' base runit elogind-runit
ENV LANG=en_US.UTF-8
CMD ["/usr/bin/runit"]
