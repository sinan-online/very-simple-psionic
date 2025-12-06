FROM ghcr.io/dante-ev/texlive:latest

RUN apt update && apt install -y git vim zsh
WORKDIR /workspace

ENV TEXINPUTS=.:/workspace/classes//:

RUN tlmgr update --self
RUN tlmgr update --all