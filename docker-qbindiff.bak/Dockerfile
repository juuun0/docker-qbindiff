FROM debian:stable-slim

RUN apt update && apt upgrade -y

RUN apt install python3.11 pipx -y
RUN pipx ensurepath

RUN pipx install qbindiff

RUN apt clean; \
    rm -rf /var/lib/apt/lists/*

# ENTRYPOINT ["/root/.local/bin/qbindiff"]
