FROM mcr.microsoft.com/devcontainers/java:1-21-bullseye

COPY --chown=vscode:vscode maven/settings.xml /home/vscode/.m2/settings.xml
RUN apt-get update -y && \
    apt-get install -y --no-install-recommends \
        libxtst6 && \
    apt-get clean -y && \
    rm -rf /var/lib/apt/lists/*
