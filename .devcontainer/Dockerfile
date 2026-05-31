FROM archlinux:base-devel
# አስፈላጊ የሆኑ መሰረታዊ መሳሪያዎችን መጫን
RUN pacman -Syu --noconfirm git vim curl sudo
# አዲስ ተጠቃሚ መፍጠር (ከroot መውጣት)
RUN useradd -m -G wheel -s /bin/bash student && \
    echo "%wheel ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
USER student
WORKDIR /home/student
