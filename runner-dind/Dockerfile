FROM summerwind/actions-runner-dind:latest

#ARG HELM_VERSION="3.7.2"

RUN set -eux; \
    curl https://baltocdn.com/helm/signing.asc | sudo apt-key add -; \
    sudo apt-get install apt-transport-https --yes; \
    echo "deb https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list; \
    sudo apt-get update; \
    sudo apt-get install helm; \
    helm version
