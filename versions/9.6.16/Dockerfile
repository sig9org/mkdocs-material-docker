FROM python:3.13.6-alpine3.22 AS build

# Build-time flags
ARG WITH_PLUGINS=true

# Environment variables
ENV PACKAGES=/usr/local/lib/python3.13/site-packages
ENV PYTHONDONTWRITEBYTECODE=1

# Set build directory
WORKDIR /tmp

# Perform build and cleanup artifacts and caches
RUN \
  apk upgrade --update-cache -a
RUN \
  apk add --no-cache \
    cairo \
    freetype-dev \
    git \
    git-fast-import \
    jpeg-dev \
    openssh \
    tini \
    zlib-dev
RUN \
  apk add --no-cache --virtual .build \
    gcc \
    g++ \
    libffi-dev \
    musl-dev
RUN \
  pip install --no-cache-dir --upgrade pip
RUN \
  pip install --no-cache-dir \
    markdown \
    mkdocs \
    mkdocs-material \
    mkdocs-material-extensions \
    mkdocs-redirects \
    mkdocs-video \
    pygments \
    pymdown-extensions
RUN \
  apk del .build
RUN \
  rm -rf /tmp/* /root/.cache

# From empty image
FROM scratch

# Copy all from build
COPY --from=build / /

# Set working directory
WORKDIR /root

# Expose MkDocs development server port
EXPOSE 8000

# Shell
CMD ["/bin/sh"]
