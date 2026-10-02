# SearXNG with our settings.yml baked in: Portainer git stacks can't bind-mount
# relative paths from the repo. The file lives outside the image's /etc/searxng
# VOLUME so changes aren't masked by a stale volume on redeploy.
ARG SEARXNG_VERSION=latest
FROM docker.io/searxng/searxng:${SEARXNG_VERSION}

COPY settings.yml /usr/local/searxng/custom/settings.yml
ENV SEARXNG_SETTINGS_PATH=/usr/local/searxng/custom/settings.yml
