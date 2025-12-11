FROM ghcr.io/dante-ev/texlive:latest

RUN apt update && apt install -y git vim zsh aspell hunspell hunspell-en-us
WORKDIR /workspace

ENV TEXINPUTS=.:/workspace/classes//:

RUN tlmgr update --self
RUN tlmgr update --all