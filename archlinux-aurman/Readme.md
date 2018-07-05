# Image

Docker image of ArchLinux with aurman installed.

# Usage

Install package from official repositories:

aurman --noconfirm -S <package>

Install package from AUR:

sudo -u aur aurman --noconfirm --noedit -S <package>

Cleanup:

pacman -Qtdq | xargs -r pacman --noconfirm -Rcns
yes | pacman -Scc
rm -rf /home/aur/.cache/aurman
