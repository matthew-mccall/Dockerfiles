FROM quay.io/fedora/fedora-minimal

RUN dnf install -y \
    texlive-scheme-full \
    kicad \
    graphviz \
    inkscape \
    plantuml

RUN luaotfload-tool --update
