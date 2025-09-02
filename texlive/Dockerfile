FROM fedora

RUN dnf install -y \
    texlive-scheme-full \
    kicad

RUN dnf install -y \
    texlive-dot2texi \
    graphviz \
    dot2tex \
    inkscape

RUN luaotfload-tool --update