FROM mcr.microsoft.com/vscode/devcontainers/universal:linux
USER root
COPY .devcontainer/components/*.sh /tmp/deploy/


RUN apt-get update && apt-get install
RUN apt-get update \
   && /bin/bash /tmp/deploy/pwsh.sh \
   && /bin/bash /tmp/deploy/dotnet.sh