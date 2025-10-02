FROM python:3.13.7-alpine3.22 AS build

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
    markdown==3.9 \
    mkdocs==1.6.1 \
    mkdocs-add-number-plugin==1.2.2 \
    mkdocs-material==9.6.19 \
    mkdocs-material-extensions==1.3.1 \
    mkdocs-redirects==1.2.2 \
    mkdocs-video==1.5.0 \
    pygments==2.19.2 \
    pymdown-extensions==10.16.1
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
