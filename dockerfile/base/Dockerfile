FROM scratch
ADD artixlinux.tar /

# manually run all alpm hooks that can't be run inside the fakechroot
RUN ldconfig && update-ca-trust && locale-gen
#RUN sh -c 'ls usr/lib/sysusers.d/*.conf | /usr/share/libalpm/scripts/sysusers-hook sysusers '

RUN sh -c 'rm -rvf /usr/share/pacman/keyring/artix.gpg'

# initialize the artix keyring, but discard any private key that may be shipped.
RUN pacman-key --init && pacman-key --populate artix



ENV LANG=en_US.UTF-8
CMD ["/usr/bin/bash"]
