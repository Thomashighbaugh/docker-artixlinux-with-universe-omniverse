FROM thighbaugh/artixlinux-with-universe-omniverse-base:latest
RUN pacman --noconfirm -Syu base openrc elogind-openrc
ENV LANG=en_US.UTF-8
CMD ["/usr/bin/openrc-init"]
