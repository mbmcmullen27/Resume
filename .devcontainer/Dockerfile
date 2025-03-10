FROM archlinux:latest
RUN pacman -Syyu base-devel texlive-fontsextra texlive-core texlive-pictures texlive-latexextra texlive-luatex texlive-fontsrecommended pdftk ttf-ibm-plex git --noconfirm && rm -r /var/cache/pacman/pkg/*
WORKDIR /usr/share/fonts/TTF
RUN for i in https://raw.github.com/googlefonts/robotoslab/master/fonts/ttf/RobotoSlab-Bold.ttf https://raw.github.com/googlefonts/robotoslab/master/fonts/ttf/RobotoSlab-ExtraBold.ttf; do curl -LJO $i; done
COPY ttf-manrope-4.505-1-any.pkg.tar .
RUN pacman -U ttf-manrope-4.505-1-any.pkg.tar --noconfirm
RUN useradd -m vscode
WORKDIR /app