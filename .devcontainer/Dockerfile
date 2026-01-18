FROM ghcr.io/dante-ev/texlive:latest

RUN apt update && apt install -y git vim zsh aspell hunspell hunspell-en-us
WORKDIR /workspace

ENV TEXINPUTS=.:/workspace/classes//:

RUN tlmgr update --self
RUN tlmgr update --all

RUN useradd -m vscode && \
    mkdir -p /home/vscode && \
    chown -R vscode:vscode /home/vscode

CMD ["/bin/bash"]