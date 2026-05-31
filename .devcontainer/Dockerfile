FROM archlinux:latest
# BlackArch key/repo setup
RUN curl -O https://blackarch.org/strap.sh && \
    chmod +x strap.sh && \
    ./strap.sh
RUN pacman -Syu --noconfirm blackarch-general blackarch-scanner
