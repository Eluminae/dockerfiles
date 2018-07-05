FROM eluminae/archlinux-aurman

RUN sudo -u aur aurman -Sy --noconfirm --noedit imapfilter && \
    yes | pacman -Scc && \
    rm -rf /home/aur/.cache/aurman
