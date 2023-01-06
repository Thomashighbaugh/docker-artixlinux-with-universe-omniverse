FROM thighbaugh/artixlinux-with-universe-omniverse-base:latest
RUN pacman --noconfirm -Syu base runit elogind-runit
ENV LANG=en_US.UTF-8
CMD ["/usr/bin/runit"]
