# Don't edit this file, user DockerfileTemplate and buildImage.sh
###############################################
FROM registry.services.alin.be/tutum/hello-world:latest
COPY localtime /etc/localtime
RUN apk add --update bash curl
HEALTHCHECK --interval=10s --timeout=10s --retries=3 CMD curl -f http://localhost/ || exit 1
