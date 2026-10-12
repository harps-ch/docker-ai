# LiteLLM with our config.yaml baked in: Portainer git stacks can't bind-mount
# relative paths from the repo (same approach as searxng/Dockerfile).
ARG LITELLM_VERSION=main-stable
FROM ghcr.io/berriai/litellm:${LITELLM_VERSION}

COPY config.yaml /app/config.yaml
